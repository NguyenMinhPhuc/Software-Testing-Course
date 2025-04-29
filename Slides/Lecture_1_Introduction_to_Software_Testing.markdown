# Bài Giảng 1: Giới Thiệu Về Kiểm Thử Phần Mềm

## Slide 1: Kiểm Thử Phần Mềm Là Gì?
**Nội dung chính**:  
- **Định nghĩa**:  
  - Kiểm thử phần mềm là quá trình đánh giá và xác minh phần mềm để đảm bảo đáp ứng yêu cầu và không có lỗi nghiêm trọng.  
  - Mục tiêu: Đảm bảo chất lượng, tính ổn định, và trải nghiệm người dùng tốt.  
- **Vai trò trong phát triển phần mềm**:  
  - Phát hiện lỗi trước khi phát hành.  
  - Đảm bảo sản phẩm đáp ứng yêu cầu khách hàng.  
**Ví dụ**:  
- Với Notepad Cải Tiến, kiểm thử đảm bảo tính năng chỉnh sửa văn bản hoạt động đúng trên Windows 10/11.  
**Hoạt động**: Thảo luận nhóm về vai trò kiểm thử trong dự án thực tế.  

---

## Slide 2: Lợi Ích Của Kiểm Thử Phần Mềm
**Nội dung chính**:  
- **Lợi ích chính**:  
  - Giảm rủi ro lỗi sau phát hành.  
  - Tăng độ tin cậy và hiệu suất phần mềm.  
  - Tiết kiệm chi phí sửa lỗi (sửa lỗi sau phát hành đắt hơn 10-100 lần).  
  - Cải thiện trải nghiệm người dùng và uy tín thương hiệu.  
- **Tầm quan trọng**:  
  - Đảm bảo phần mềm hoạt động đúng trong các tình huống thực tế.  
**Ví dụ**:  
- Kiểm thử Notepad Cải Tiến giúp phát hiện lỗi xuất báo cáo chậm, tránh ảnh hưởng đến QA.  
**Hoạt động**: Liệt kê 3 lợi ích kiểm thử cho một ứng dụng giả định (ví dụ: ứng dụng ghi chú).  

---

## Slide 3: Các Phương Pháp Kiểm Thử
**Nội dung chính**:  
- **Phân loại theo cách thực hiện**:  
  - **Kiểm thử thủ công**: QA thực hiện test case bằng tay.  
  - **Kiểm thử tự động**: Dùng công cụ/script để tự động hóa.  
- **Phân loại theo cách tiếp cận**:  
  - **Hộp đen (Black-box)**: Chỉ kiểm tra đầu vào/đầu ra, không quan tâm code.  
  - **Hộp trắng (White-box)**: Kiểm tra dựa trên cấu trúc code.  
  - **Hộp xám (Grey-box)**: Kết hợp cả hai.  
- **Phân loại theo cấp độ**:  
  - Kiểm thử đơn vị, tích hợp, hệ thống, chấp nhận.  
**Ví dụ**:  
- Notepad Cải Tiến dùng kiểm thử thủ công hộp đen để kiểm tra tìm kiếm nâng cao.  
**Hoạt động**: Sinh viên phân loại các phương pháp kiểm thử cho một tính năng cụ thể.  

---

## Slide 4: Khi Nào Dùng Kiểm Thử Thủ Công?
**Nội dung chính**:  
- **Ưu điểm kiểm thử thủ công**:  
  - Phù hợp với các dự án nhỏ, yêu cầu thay đổi thường xuyên.  
  - Tốt cho kiểm thử giao diện người dùng và trải nghiệm người dùng.  
  - Không cần đầu tư công cụ phức tạp.  
- **Nhược điểm**:  
  - Tốn thời gian, dễ bỏ sót lỗi.  
  - Không hiệu quả cho kiểm thử lặp lại hoặc dữ liệu lớn.  
- **Trường hợp sử dụng**:  
  - Kiểm thử tính năng mới, kiểm thử chấp nhận, hoặc dự án ngắn hạn.  
**Ví dụ**:  
- Notepad Cải Tiến: Kiểm thử thủ công để xác minh giao diện và xuất báo cáo.  
**Hoạt động**: Thảo luận khi nào nên dùng kiểm thử thủ công thay vì tự động.
---
#### Slide 5: Ví Dụ Thực Tế - Kiểm Thử Todo App
**Nội dung chính**:  
- **Dự án**: Todo App (ứng dụng web quản lý công việc).  
- **Tính năng chính**: Tạo công việc, gắn thẻ ưu tiên, lọc theo trạng thái (hoàn thành/chưa hoàn thành).  
- **Kiểm thử thủ công**:  
  - Kiểm tra giao diện nhập công việc.  
  - Xác minh chức năng lọc công việc.  
**Ví dụ**:  
- Kiểm thử nhập công việc với tiêu đề dài (>100 ký tự) để phát hiện lỗi giao diện.  
**Hoạt động**: Thảo luận vai trò kiểm thử thủ công trong Todo App so với Notepad Cải Tiến.  

---

#### Slide 6: Lợi Ích Kiểm Thử Trong Todo App
**Nội dung chính**:  
- **Lợi ích cụ thể**:  
  - Phát hiện lỗi hiển thị trạng thái công việc sai (ví dụ: công việc hoàn thành vẫn hiển thị "chưa hoàn thành").  
  - Đảm bảo tương thích với các trình duyệt (Chrome, Firefox).  
  - Tăng trải nghiệm người dùng khi lọc công việc nhanh chóng.  
**Ví dụ**:  
- Kiểm thử giúp tiết kiệm chi phí sửa lỗi giao diện trên nhiều thiết bị.  
**Hoạt động**: Liệt kê 3 lợi ích kiểm thử cho Todo App.  

---

#### Slide 7: Phương Pháp Kiểm Thử Áp Dụng Cho Todo App
**Nội dung chính**:  
- **Kiểm thử thủ công hộp đen**:  
  - Kiểm tra chức năng tạo công việc mà không cần biết code.  
- **Kiểm thử tích hợp**:  
  - Xác minh tương tác giữa giao diện và cơ sở dữ liệu (công việc lưu đúng).  
- **Kiểm thử chấp nhận**:  
  - Đảm bảo người dùng cuối hài lòng với chức năng lọc.  
**Ví dụ**:  
- Kiểm thử hộp đen: Nhập công việc, kiểm tra hiển thị đúng trên danh sách.  
**Hoạt động**: Phân loại phương pháp kiểm thử cho tính năng lọc công việc.  

---

#### Slide 8: Kiểm Thử Thủ Công Trong Todo App
**Nội dung chính**:  
- **Ứng dụng kiểm thử thủ công**:  
  - Kiểm tra trải nghiệm người dùng khi thêm công việc (dễ sử dụng, trực quan).  
  - Kiểm tra lỗi giao diện trên các độ phân giải màn hình khác nhau.  
- **Ưu điểm**:  
  - Phát hiện lỗi trực quan mà kiểm thử tự động khó nhận ra.  
**Ví dụ**:  
- Kiểm tra nút "Xóa công việc" có hiển thị rõ trên màn hình nhỏ.  
**Hoạt động**: Thảo luận trường hợp nào trong Todo App cần kiểm thử thủ công.  

---

#### Slide 9: Thách Thức Kiểm Thử Trong Todo App
**Nội dung chính**:  
- **Thách thức**:  
  - Kiểm thử trên nhiều trình duyệt và thiết bị (desktop, mobile).  
  - Xử lý dữ liệu công việc lớn (hàng nghìn công việc).  
- **Giải pháp**:  
  - Sử dụng checklist kiểm thử trình duyệt.  
  - Mô phỏng dữ liệu lớn để kiểm tra hiệu suất.  
**Ví dụ**:  
- Phát hiện lỗi chậm khi lọc 1,000 công việc qua kiểm thử thủ công.  
**Hoạt động**: Đề xuất cách khắc phục thách thức kiểm thử trong Todo App.  
---