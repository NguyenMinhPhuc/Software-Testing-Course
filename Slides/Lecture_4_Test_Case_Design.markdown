# Bài Giảng 4: Test Case và Cách Xây Dựng

## Slide 1: Test Case Là Gì?
**Nội dung chính**:  
- **Định nghĩa**:  
  - Tài liệu chi tiết mô tả cách kiểm thử một yêu cầu, bao gồm bước thực hiện và kết quả mong đợi.  
  - Là công cụ chính trong kiểm thử thủ công.  
- **Mục đích**:  
  - Xác minh tính năng hoạt động đúng.  
  - Phát hiện lỗi và báo cáo kết quả.  
**Ví dụ**:  
- Notepad Cải Tiến: TC-001 kiểm tra tạo và chỉnh sửa ghi chú.  
**Hoạt động**: Thảo luận vai trò của test case trong kiểm thử thủ công.  

---

## Slide 2: Cấu Trúc Test Case
**Nội dung chính**:  
- **ID**: Mã định danh (TC-001).  
- **Mô tả**: Mục tiêu kiểm thử (ví dụ: Kiểm tra lưu file).  
- **Điều kiện tiên quyết**: Trạng thái ban đầu (ứng dụng đã cài).  
- **Bước thực hiện**: Các bước cụ thể (nhập văn bản, nhấn Save).  
- **Kết quả mong đợi**: Kết quả đúng (file được lưu).  
- **Kết quả thực tế**: Pass/Fail sau kiểm thử.  
**Ví dụ**:  
- TC-002 (Notepad Cải Tiến): Lưu file .txt, kết quả là file xuất hiện trên Desktop.  
**Hoạt động**: Sinh viên liệt kê cấu trúc test case cho một tính năng giả định.  

---

## Slide 3: Cách Xây Dựng Test Case
**Nội dung chính**:  
- **Bước 1**: Dựa trên yêu cầu kiểm thử (TR) từ PRD.  
- **Bước 2**: Xác định các trường hợp:  
  - Bình thường: Trường hợp sử dụng thông thường.  
  - Lỗi: Trường hợp thất bại (ví dụ: lưu vào thư mục khóa).  
  - Biên: Giới hạn (ví dụ: file 10MB).  
- **Bước 3**: Viết rõ ràng, ngắn gọn, đảm bảo bao phủ yêu cầu.  
- **Bước 4**: Kiểm tra tính khả thi (có thể thực thi).  
**Ví dụ**:  
- TC-006 (Notepad Cải Tiến): Tìm kiếm theo thẻ "Lỗi", kiểm tra trường hợp không có kết quả.  
**Hoạt động**: Sinh viên viết 3 test case cho tính năng tìm kiếm nâng cao của Notepad Cải Tiến.  

---

## Slide 4: Lưu Ý Khi Thiết Kế Test Case
**Nội dung chính**:  
- **Đầy đủ**: Bao phủ tất cả yêu cầu và trường hợp.  
- **Rõ ràng**: Dễ hiểu cho QA và các bên liên quan.  
- **Khả thi**: Có thể thực thi trong môi trường kiểm thử.  
- **Bảo trì**: Dễ cập nhật khi yêu cầu thay đổi.  
**Ví dụ**:  
- Notepad Cải Tiến: Test case xuất báo cáo cần kiểm tra cả CSV và TXT.  
**Hoạt động**: Thảo luận cách tối ưu test case để giảm thời gian thực thi.  

---

## Slide 5: Thách Thức Khi Xây Dựng Test Case
**Nội dung chính**:  
- **Yêu cầu không rõ**: Dẫn đến test case thiếu sót.  
- **Quá nhiều test case**: Tốn thời gian thực thi.  
- **Thay đổi yêu cầu**: Test case cần cập nhật thường xuyên.  
- **Giải pháp**:  
  - Phối hợp chặt chẽ với đội phát triển.  
  - Sử dụng công cụ quản lý test case (TestRail).  
**Ví dụ**:  
- Notepad Cải Tiến: Test case xuất báo cáo phải cập nhật khi thêm định dạng mới.  
**Hoạt động**: Sinh viên đề xuất cách quản lý test case hiệu quả trong dự án lớn.  

---

## Slide 6: Ví Dụ Thực Tế - Test Case Cho Todo App
**Nội dung chính**:  
- **Dự án**: Todo App (web).  
- **Test Case**:  
  - Kiểm tra tạo công việc với tiêu đề hợp lệ.  
  - Kiểm tra lọc công việc theo trạng thái "hoàn thành".  
- **Cấu trúc**: ID, mô tả, bước thực hiện, kết quả mong đợi.  
**Ví dụ**:  
- TC-001: Tạo công việc, nhập tiêu đề "Họp nhóm", kết quả hiển thị trong danh sách.  
**Hoạt động**: Thảo luận test case của Todo App so với Notepad Cải Tiến.  

---

## Slide 7: Xây Dựng Test Case Trong Todo App
**Nội dung chính**:  
- **Dựa trên TR**: TR-001 (Tạo công việc) dẫn đến TC-001.  
- **Trường hợp**:  
  - Bình thường: Tạo công việc với tiêu đề hợp lệ.  
  - Lỗi: Tạo công việc với tiêu đề rỗng.  
  - Biên: Tiêu đề 200 ký tự.  
**Ví dụ**:  
- TC-002: Kiểm tra lỗi khi tạo công việc với tiêu đề rỗng, mong đợi thông báo lỗi.  
**Hoạt động**: Sinh viên viết 3 test case cho tính năng lọc công việc.  

---

## Slide 8: Lưu Ý Test Case Trong Todo App
**Nội dung chính**:  
- **Đầy đủ**: Bao phủ tạo, xóa, lọc công việc.  
- **Rõ ràng**: Bước thực hiện dễ hiểu (nhấn nút "Thêm").  
- **Khả thi**: Kiểm tra trên Chrome/Firefox.  
**Ví dụ**:  
- TC-003: Lọc công việc "hoàn thành", kiểm tra trên Chrome, kết quả chính xác.  
**Hoạt động**: Thảo luận cách đảm bảo test case rõ ràng trong Todo App.  

---

## Slide 9: Thách Thức Test Case Trong Todo App
**Nội dung chính**:  
- **Yêu cầu thay đổi**: Thêm trạng thái "đang xử lý" cần cập nhật test case.  
- **Dữ liệu lớn**: Kiểm tra lọc 1,000 công việc tốn thời gian.  
- **Giải pháp**:  
  - Sử dụng TestRail để quản lý test case.  
  - Tối ưu test case cho trường hợp biên.  
**Ví dụ**:  
- Todo App: TC-004 cập nhật để kiểm tra lọc trạng thái mới.  
**Hoạt động**: Đề xuất cách quản lý test case trong Todo App.  

---

## Slide 10: Kiểm Tra Test Case Trong Todo App
**Nội dung chính**:  
- **Quy trình kiểm tra**:  
  - Đánh giá tính đầy đủ (bao phủ TR).  
  - Xác minh tính khả thi (môi trường kiểm thử).  
- **Lợi ích**:  
  - Đảm bảo test case thực thi hiệu quả, không dư thừa.  
**Ví dụ**:  
- Todo App: Kiểm tra TC-001 để đảm bảo bao phủ TR-001 (tạo công việc).  
**Hoạt động**: Sinh viên đánh giá một test case giả định cho Todo App.