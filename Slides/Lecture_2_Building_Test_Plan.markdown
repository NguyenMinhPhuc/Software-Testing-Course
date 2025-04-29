# Bài Giảng 2: Xây Dựng Test Plan

## Slide 1: Test Plan Là Gì?
**Nội dung chính**:  
- **Định nghĩa**:  
  - Tài liệu mô tả chiến lược, phạm vi, tài nguyên, và lịch trình kiểm thử.  
  - Là kim chỉ nam cho quá trình kiểm thử, đảm bảo có hệ thống và hiệu quả.  
- **Mục đích**:  
  - Xác định mục tiêu kiểm thử.  
  - Đảm bảo bao phủ yêu cầu và quản lý rủi ro.  
**Ví dụ**:  
- Test Plan của Notepad Cải Tiến xác định kiểm thử chỉnh sửa văn bản, tìm kiếm nâng cao trên Windows 10/11.  
**Hoạt động**: Thảo luận vai trò của Test Plan trong dự án phần mềm.  

---

## Slide 2: Các Thành Phần Của Test Plan
**Nội dung chính**:  
- **Phạm vi (Scope)**: Tính năng kiểm thử (trong/ngoài phạm vi).  
- **Mục tiêu chất lượng**: Đáp ứng PRD, không có lỗi nghiêm trọng.  
- **Phương pháp kiểm thử**: Agile, Waterfall, v.v.  
- **Vai trò và trách nhiệm**: QA, nhà phát triển, quản lý dự án.  
- **Tài nguyên**: Công cụ (TestRail, Bugzilla), môi trường (Windows).  
- **Tiêu chí hoàn thành**: 95% bao phủ, lỗi nghiêm trọng được sửa.  
**Ví dụ**:  
- Notepad Cải Tiến: Phạm vi bao gồm kiểm thử xuất báo cáo, ngoài phạm vi là đồng bộ đám mây.  
**Hoạt động**: Liệt kê các thành phần của Test Plan cho một ứng dụng giả định.  

---

## Slide 3: Quy Trình Lập Test Plan
**Nội dung chính**:  
- **Bước 1**: Phân tích PRD để xác định yêu cầu kiểm thử.  
- **Bước 2**: Xác định phạm vi kiểm thử (tính năng, yêu cầu chức năng/phi chức năng).  
- **Bước 3**: Lựa chọn phương pháp kiểm thử (Agile, Waterfall).  
- **Bước 4**: Xác định tài nguyên (công cụ, môi trường, nhân sự).  
- **Bước 5**: Định nghĩa tiêu chí tạm dừng/tiếp tục và hoàn thành.  
**Ví dụ**:  
- Notepad Cải Tiến: Test Plan dùng Agile, kiểm thử trên Windows 10/11, tiêu chí hoàn thành là 95% bao phủ.  
**Hoạt động**: Sinh viên lập Test Plan cơ bản cho ứng dụng giả định (ví dụ: ứng dụng To-Do List).  

---

## Slide 4: Lưu Ý Khi Lập Test Plan
**Nội dung chính**:  
- **Rõ ràng và cụ thể**: Phạm vi, mục tiêu phải dễ hiểu.  
- **Linh hoạt**: Dễ điều chỉnh khi yêu cầu thay đổi.  
- **Hợp tác**: Phối hợp với các bên liên quan (QA, nhà phát triển, quản lý).  
- **Tập trung vào rủi ro**: Xác định rủi ro (hiệu suất, tương thích) và kế hoạch giảm thiểu.  
**Ví dụ**:  
- Notepad Cải Tiến: Rủi ro hiệu suất với 10,000 ghi chú, giảm thiểu bằng tối ưu SQLite.  
**Hoạt động**: Thảo luận các rủi ro tiềm ẩn khi lập Test Plan cho một dự án.  

---

## Slide 5: Ví Dụ Thực Tế - Test Plan Cho Todo App
**Nội dung chính**:  
- **Dự án**: Todo App (web).  
- **Test Plan**:  
  - **Phạm vi**: Kiểm thử tạo/xóa công việc, lọc theo trạng thái.  
  - **Ngoài phạm vi**: Tích hợp với Google Calendar.  
  - **Phương pháp**: Agile, kiểm thử thủ công hộp đen.  
**Ví dụ**:  
- Test Plan xác định kiểm thử trên Chrome/Firefox, không bao gồm Safari.  
**Hoạt động**: Thảo luận phạm vi kiểm thử của Todo App so với Notepad Cải Tiến.  

---

## Slide 6: Thành Phần Test Plan Trong Todo App
**Nội dung chính**:  
- **Phạm vi**: Tạo, chỉnh sửa, xóa công việc; tương thích trình duyệt.  
- **Mục tiêu chất lượng**: Không có lỗi nghiêm trọng, lọc công việc < 1 giây.  
- **Tài nguyên**: Công cụ TestRail, môi trường web (Chrome, Firefox).  
- **Tiêu chí hoàn thành**: 90% test case passed, lỗi cao được sửa.  
**Ví dụ**:  
- Todo App yêu cầu kiểm thử trên cấu hình tối thiểu (4GB RAM, Windows 10).  
**Hoạt động**: Liệt kê thành phần Test Plan cho Todo App.  

---

## Slide 7: Quy Trình Lập Test Plan Cho Todo App
**Nội dung chính**:  
- **Bước 1**: Phân tích PRD (tạo công việc, lọc trạng thái).  
- **Bước 2**: Xác định phạm vi (chức năng, trình duyệt).  
- **Bước 3**: Chọn Agile để kiểm thử từng sprint.  
- **Bước 4**: Sử dụng TestRail và môi trường trình duyệt.  
- **Bước 5**: Tiêu chí: 90% bao phủ, lỗi nghiêm trọng sửa ngay.  
**Ví dụ**:  
- Todo App: Test Plan yêu cầu kiểm thử 500 công việc để đánh giá hiệu suất.  
**Hoạt động**: Sinh viên lập Test Plan cơ bản cho Todo App.  

---

## Slide 8: Rủi Ro Trong Test Plan Todo App
**Nội dung chính**:  
- **Rủi ro**:  
  - Tương thích trình duyệt (lỗi hiển thị trên Firefox).  
  - Hiệu suất khi xử lý dữ liệu lớn.  
- **Giảm thiểu**:  
  - Kiểm thử trên nhiều trình duyệt từ sớm.  
  - Mô phỏng dữ liệu lớn trong môi trường kiểm thử.  
**Ví dụ**:  
- Test Plan dự đoán rủi ro chậm khi lọc công việc, yêu cầu tối ưu API.  
**Hoạt động**: Thảo luận rủi ro kiểm thử trong Todo App.  

---

## Slide 9: Linh Hoạt Trong Test Plan Todo App
**Nội dung chính**:  
- **Tính linh hoạt**:  
  - Dễ cập nhật khi thêm tính năng (ví dụ: gắn thẻ ưu tiên).  
  - Điều chỉnh lịch trình kiểm thử khi sprint thay đổi.  
- **Cách thực hiện**:  
  - Sử dụng tài liệu sống (Google Docs, TestRail).  
  - Họp định kỳ để cập nhật Test Plan.  
**Ví dụ**:  
- Todo App: Test Plan cập nhật khi thêm yêu cầu lọc theo ưu tiên.  
**Hoạt động**: Đề xuất cách giữ Test Plan linh hoạt trong dự án web.