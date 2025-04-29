# Bài Giảng 5: Thực Hiện Báo Cáo Kiểm Thử

## Slide 1: Test Report Là Gì?
**Nội dung chính**:  
- **Định nghĩa**:  
  - Tài liệu tổng hợp kết quả kiểm thử, trạng thái lỗi, và đánh giá chất lượng ứng dụng.  
  - Dùng để báo cáo cho các bên liên quan (QA, nhà phát triển, quản lý).  
- **Mục đích**:  
  - Truyền đạt trạng thái kiểm thử.  
  - Đưa ra quyết định phát hành hoặc sửa lỗi.  
**Ví dụ**:  
- Test Report của Notepad Cải Tiến: 85.7% test case passed, 2 lỗi cần sửa.  
**Hoạt động**: Thảo luận vai trò của Test Report trong dự án phần mềm.  

---

## Slide 2: Các Thành Phần Của Test Report
**Nội dung chính**:  
- **Thông tin chung**: Tên dự án, phiên bản, ngày kiểm thử.  
- **Tóm tắt kết quả**: Số test case, tỷ lệ pass/fail, bao phủ yêu cầu.  
- **Phân tích lỗi**: Danh sách lỗi, mức độ, trạng thái (đã sửa/chưa sửa).  
- **Ma trận truy xuất**: Xác nhận yêu cầu được kiểm thử.  
- **Đánh giá và khuyến nghị**: Chất lượng ứng dụng, hành động tiếp theo.  
**Ví dụ**:  
- Notepad Cải Tiến: Báo cáo nêu lỗi lọc ngày và khuyến nghị sửa trước phát hành.  
**Hoạt động**: Sinh viên liệt kê các thành phần cần có trong Test Report.  

---

## Slide 3: Quy Trình Lập Test Report
**Nội dung chính**:  
- **Bước 1**: Thu thập kết quả từ test case (pass/fail).  
- **Bước 2**: Tổng hợp lỗi từ công cụ theo dõi (Bugzilla, Jira).  
- **Bước 3**: Đánh giá bao phủ yêu cầu qua ma trận truy xuất.  
- **Bước 4**: Viết đánh giá và khuyến nghị (sửa lỗi, kiểm thử bổ sung).  
- **Bước 5**: Phê duyệt bởi quản lý kiểm thử.  
**Ví dụ**:  
- Notepad Cải Tiến: Báo cáo tổng hợp 14 test case, 5 lỗi, phê duyệt ngày 13/05/2025.  
**Hoạt động**: Sinh viên lập Test Report giả định cho 5 test case.  

---

## Slide 4: Lưu Ý Khi Lập Test Report
**Nội dung chính**:  
- **Rõ ràng**: Trình bày ngắn gọn, dễ hiểu.  
- **Chính xác**: Dữ liệu phải đúng (số test case, lỗi).  
- **Hữu ích**: Đưa ra khuyến nghị khả thi (sửa lỗi, kiểm thử lại).  
- **Kịp thời**: Gửi báo cáo đúng hạn để hỗ trợ quyết định phát hành.  
**Ví dụ**:  
- Notepad Cải Tiến: Báo cáo khuyến nghị sửa lỗi múi giờ trước phát hành.  
**Hoạt động**: Thảo luận cách trình bày Test Report để thuyết phục các bên liên quan.  

---

## Slide 5: Thách Thức Khi Lập Test Report
**Nội dung chính**:  
- **Dữ liệu không đầy đủ**: Thiếu kết quả test case hoặc thông tin lỗi.  
- **Áp lực thời gian**: Báo cáo cần hoàn thành nhanh trước phát hành.  
- **Mâu thuẫn ý kiến**: Các bên liên quan không đồng ý về lỗi ưu tiên.  
- **Giải pháp**:  
  - Sử dụng công cụ quản lý kiểm thử (TestRail).  
  - Họp phân loại lỗi (bug triage) để thống nhất.  
**Ví dụ**:  
- Notepad Cải Tiến: Thách thức khi báo cáo lỗi hiệu suất do thiếu dữ liệu kiểm thử lớn.  
**Hoạt động**: Sinh viên đề xuất cách cải thiện quy trình lập Test Report.  

---

## Slide 6: Ví Dụ Thực Tế - Test Report Cho Todo App
**Nội dung chính**:  
- **Dự án**: Todo App (web).  
- **Test Report**:  
  - Tổng hợp kết quả kiểm thử tạo, xóa, lọc công việc.  
  - Báo cáo lỗi giao diện và hiệu suất.  
**Ví dụ**:  
- Test Report: 90% test case passed, 2 lỗi giao diện trên Firefox cần sửa.  
**Hoạt động**: Thảo luận Test Report của Todo App so với Notepad Cải Tiến.  

---

## Slide 7: Thành Phần Test Report Trong Todo App
**Nội dung chính**:  
- **Thông tin chung**: Phiên bản 1.0, kiểm thử 01/06/2025.  
- **Tóm tắt**: 20 test case, 90% passed, 95% bao phủ.  
- **Lỗi**: 3 lỗi (1 cao, 2 thấp), 1 lỗi chưa sửa.  
- **Khuyến nghị**: Sửa lỗi trước phát hành.  
**Ví dụ**:  
- Todo App: Báo cáo nêu lỗi chậm khi lọc 1,000 công việc.  
**Hoạt động**: Liệt kê thành phần Test Report cho Todo App.  

---

## Slide 8: Quy Trình Test Report Trong Todo App
**Nội dung chính**:  
- **Thu thập**: Kết quả test case từ TestRail.  
- **Tổng hợp lỗi**: Sử dụng Jira để theo dõi.  
- **Đánh giá**: Kiểm tra bao phủ qua ma trận truy xuất.  
- **Khuyến nghị**: Sửa lỗi hiệu suất và kiểm thử lại.  
**Ví dụ**:  
- Todo App: Báo cáo đề xuất tối ưu API lọc công việc.  
**Hoạt động**: Sinh viên lập Test Report giả định cho 5 test case của Todo App.  

---

## Slide 9: Lưu Ý Test Report Trong Todo App
**Nội dung chính**:  
- **Chính xác**: Số test case và lỗi phải đúng.  
- **Hữu ích**: Khuyến nghị cụ thể (sửa lỗi, kiểm tra trình duyệt).  
- **Kịp thời**: Gửi trước hạn phát hành.  
**Ví dụ**:  
- Todo App: Báo cáo nêu lỗi giao diện, đề xuất kiểm tra trên mobile.  
**Hoạt động**: Thảo luận cách làm Test Report thuyết phục trong Todo App.  

---

## Slide 10: Thách Thức Test Report Trong Todo App
**Nội dung chính**:  
- **Dữ liệu thiếu**: Kết quả kiểm thử trình duyệt chưa đầy đủ.  
- **Áp lực thời gian**: Báo cáo cần hoàn thành trong 1 ngày.  
- **Giải pháp**:  
  - Sử dụng mẫu báo cáo chuẩn.  
  - Tự động hóa thu thập dữ liệu từ TestRail.  
**Ví dụ**:  
- Todo App: Thách thức khi báo cáo lỗi hiệu suất do thiếu dữ liệu lớn.  
**Hoạt động**: Đề xuất cách cải thiện Test Report cho Todo App.