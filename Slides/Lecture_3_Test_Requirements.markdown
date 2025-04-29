# Bài Giảng 3: Xác Định Yêu Cầu Kiểm Thử

## Slide 1: Yêu Cầu Kiểm Thử Là Gì?
**Nội dung chính**:  
- **Định nghĩa**:  
  - Các điều kiện hoặc tính năng cần kiểm thử, dựa trên PRD.  
  - Là nền tảng để xây dựng test case và đảm bảo bao phủ yêu cầu.  
- **Loại yêu cầu**:  
  - **Chức năng**: Tính năng cụ thể (tạo file, tìm kiếm).  
  - **Phi chức năng**: Hiệu suất, bảo mật, tương thích.  
**Ví dụ**:  
- Notepad Cải Tiến: TR-001 (Tạo ghi chú), TR-015 (Mã hóa AES-256).  
**Hoạt động**: Thảo luận sự khác biệt giữa yêu cầu chức năng và phi chức năng.  

---

## Slide 2: Cách Xác Định Yêu Cầu Kiểm Thử
**Nội dung chính**:  
- **Bước 1**: Đọc và phân tích PRD để liệt kê tính năng.  
- **Bước 2**: Phân loại yêu cầu (chức năng/phi chức năng).  
- **Bước 3**: Gán ID và mô đánh rõ ràng (ví dụ: TR-002: Lưu file .txt).  
- **Bước 4**: Xác minh với các bên liên quan (QA, khách hàng).  
**Ví dụ**:  
- Notepad Cải Tiến: TR-010 (Tìm kiếm theo thẻ), yêu cầu hiệu suất < 0,5 giây.  
**Hoạt động**: Sinh viên phân tích PRD của Notepad Cải Tiến và liệt kê 5 yêu cầu kiểm thử.  

---

## Slide 3: Tầm Quan Trọng Của Yêu Cầu Kiểm Thử
**Nội dung chính**:  
- **Đảm bảo bao phủ**: Mọi tính năng trong PRD đều được kiểm thử.  
- **Cơ sở cho test case**: Hướng dẫn thiết kế test case chi tiết.  
- **Hỗ trợ ma trận truy xuất**: Liên kết yêu cầu với kết quả kiểm thử.  
- **Giảm rủi ro**: Phát hiện thiếu sót yêu cầu sớm.  
**Ví dụ**:  
- Notepad Cải Tiến: TR-012 (Xuất CSV) đảm bảo báo cáo QA đầy đủ thông tin.  
**Hoạt động**: Thảo luận hậu quả nếu bỏ sót yêu cầu kiểm thử trong dự án.  

---

## Slide 4: Thách Thức Khi Xác Định Yêu Cầu
**Nội dung chính**:  
- **Yêu cầu không rõ ràng**: PRD thiếu chi tiết hoặc mâu thuẫn.  
- **Thay đổi yêu cầu**: Khách hàng thay đổi trong quá trình phát triển.  
- **Thiếu thông tin**: Không đủ dữ liệu về môi trường sử dụng.  
- **Giải pháp**:  
  - Họp xác minh yêu cầu với khách hàng.  
  - Sử dụng checklist yêu cầu kiểm thử.  
**Ví dụ**:  
- Notepad Cải Tiến: Yêu cầu xuất báo cáo ban đầu không rõ định dạng (CSV/TXT).  
**Hoạt động**: Sinh viên đề xuất cách xử lý yêu cầu mập mờ trong PRD.  

---

## Slide 5: Ví Dụ Thực Tế - Yêu Cầu Kiểm Thử Todo App
**Nội dung chính**:  
- **Dự án**: Todo App (web).  
- **Yêu cầu kiểm thử**:  
  - **Chức năng**: Tạo/xóa công việc, lọc theo trạng thái.  
  - **Phi chức năng**: Hiệu suất lọc < 1 giây, tương thích Chrome/Firefox.  
**Ví dụ**:  
- TR-001: Người dùng có thể tạo công việc với tiêu đề tối đa 200 ký tự.  
**Hoạt động**: Thảo luận yêu cầu kiểm thử của Todo App so với Notepad Cải Tiến.  

---

## Slide 6: Xác Định Yêu Cầu Trong Todo App
**Nội dung chính**:  
- **Phân tích PRD**: Liệt kê tính năng (tạo công việc, lọc trạng thái).  
- **Phân loại**:  
  - Chức năng: Thêm công việc, xóa công việc.  
  - Phi chức năng: Tương thích trình duyệt, hiệu suất.  
- **Gán ID**: TR-002 (Lọc công việc theo trạng thái).  
**Ví dụ**:  
- TR-003: Xóa công việc, yêu cầu xác nhận trước khi xóa.  
**Hoạt động**: Sinh viên liệt kê 5 yêu cầu kiểm thử cho Todo App.  

---

## Slide 7: Tầm Quan Trọng Yêu Cầu Trong Todo App
**Nội dung chính**:  
- **Bao phủ**: Đảm bảo mọi tính năng (tạo, lọc, xóa) được kiểm thử.  
- **Hỗ trợ test case**: TR-001 dẫn đến test case kiểm tra nhập công việc.  
- **Giảm rủi ro**: Phát hiện thiếu sót (ví dụ: thiếu yêu cầu tương thích mobile).  
**Ví dụ**:  
- Todo App: TR-004 (Tương thích Firefox) giúp phát hiện lỗi giao diện.  
**Hoạt động**: Thảo luận hậu quả nếu bỏ sót yêu cầu trong Todo App.  

---

## Slide 8: Thách Thức Yêu Cầu Trong Todo App
**Nội dung chính**:  
- **Yêu cầu mập mờ**: PRD không rõ về giới hạn tiêu đề công việc.  
- **Thay đổi**: Thêm yêu cầu lọc theo ưu tiên giữa dự án.  
- **Giải pháp**:  
  - Họp xác minh với khách hàng.  
  - Sử dụng checklist yêu cầu.  
**Ví dụ**:  
- Todo App: Yêu cầu lọc ban đầu không rõ về trạng thái "đang xử lý".  
**Hoạt động**: Đề xuất cách xử lý yêu cầu không rõ trong Todo App.  

---

## Slide 9: Xác Minh Yêu Cầu Trong Todo App
**Nội dung chính**:  
- **Quy trình xác minh**:  
  - Gửi danh sách yêu cầu cho khách hàng/đội phát triển.  
  - Sử dụng bảng câu hỏi (ví dụ: Giới hạn dữ liệu công việc?).  
- **Lợi ích**:  
  - Đảm bảo yêu cầu chính xác trước khi viết test case.  
**Ví dụ**:  
- Todo App: Xác minh TR-002 (lọc trạng thái) để bao gồm cả trạng thái rỗng.  
**Hoạt động**: Sinh viên đề xuất bảng câu hỏi xác minh yêu cầu cho Todo App.