# Bài Tập Thực Hành

## Phần 1: Bài Tập Thực Hành

Dưới đây là tài liệu bài tập thực hành cho sinh viên, dựa trên nội dung các slide, sử dụng **ứng dụng quản lý công việc (Todo App)** làm bối cảnh. Các bài tập được thiết kế để củng cố kiến thức về Test Plan, Test Case, và Test Report.

### Bài Tập Thực Hành: Kiểm Thử Thủ Công Cho Todo App

#### Giới thiệu
- **Ứng dụng**: Todo App (web) cho phép người dùng tạo, chỉnh sửa, xóa công việc, gắn thẻ ưu tiên, và lọc công việc theo trạng thái (hoàn thành/chưa hoàn thành).  
- **Mục tiêu**: Áp dụng kiến thức từ các bài giảng để lập Test Plan, viết Test Case, và tạo Test Report.  

#### Bài Tập 1: Lập Test Plan
**Mô tả**:  
- Dựa trên PRD giả định của Todo App (tính năng: tạo/xóa công việc, lọc trạng thái, tương thích Chrome/Firefox), lập Test Plan cơ bản.  
**Yêu cầu**:  
- Bao gồm:  
  - Phạm vi (trong/ngoài phạm vi).  
  - Mục tiêu chất lượng (ví dụ: 90% test case passed).  
  - Phương pháp kiểm thử (Agile, thủ công).  
  - Tài nguyên (công cụ, môi trường).  
  - Tiêu chí hoàn thành.  
- Sử dụng mẫu từ slide Lecture_2_Building_Test_Plan.  
**Hướng dẫn**:  
- Xem Slide 2, 3 (Lecture_2) để xác định thành phần và quy trình.  
- Ví dụ: Phạm vi kiểm thử bao gồm tạo công việc, ngoài phạm vi là tích hợp Google Calendar.  
**Nộp bài**: File markdown hoặc Word chứa Test Plan.  

---

#### Bài Tập 2: Viết Test Case
**Mô tả**:  
- Dựa trên các yêu cầu kiểm thử (TR) giả định cho Todo App, viết 5 test case chi tiết cho tính năng **tạo công việc** và **lọc công việc**.  
**Yêu cầu kiểm thử (TR)**:  
- TR-001: Tạo công việc với tiêu đề tối đa 200 ký tự.  
- TR-002: Xóa công việc, yêu cầu xác nhận trước khi xóa.  
- TR-003: Lọc công việc theo trạng thái "hoàn thành".  
**Yêu cầu**:  
- Mỗi test case bao gồm:  
  - ID, mô tả, điều kiện tiên quyết, bước thực hiện, kết quả mong đợi.  
- Bao phủ: Trường hợp bình thường, lỗi, biên (ví dụ: tiêu đề rỗng, 200 ký tự).  
- Sử dụng mẫu từ slide Lecture_4_Test_Case_Design.  
**Hướng dẫn**:  
- Xem Slide 2, 3 (Lecture_4) để hiểu cấu trúc và cách xây dựng test case.  
- Ví dụ: TC-001 kiểm tra tạo công việc với tiêu đề "Họp nhóm".  
**Nộp bài**: File markdown hoặc Word chứa 5 test case.  

---

#### Bài Tập 3: Lập Test Report
**Mô tả**:  
- Giả định bạn đã thực thi 5 test case từ Bài Tập 2 và có kết quả như sau:  
  - 4 test case passed, 1 test case failed (lọc công việc chậm với 1,000 công việc).  
  - Phát hiện 2 lỗi: 1 lỗi cao (hiệu suất lọc), 1 lỗi thấp (giao diện lệch).  
- Lập Test Report dựa trên kết quả này.  
**Yêu cầu**:  
- Bao gồm:  
  - Thông tin chung (dự án, ngày kiểm thử).  
  - Tóm tắt kết quả (số test case, tỷ lệ pass/fail).  
  - Phân tích lỗi (ID, mô tả, mức độ, trạng thái).  
  - Khuyến nghị (sửa lỗi, kiểm thử lại).  
- Sử dụng mẫu từ slide Lecture_5_Test_Report.  
**Hướng dẫn**:  
- Xem Slide 2, 3 (Lecture_5) để hiểu thành phần và quy trình Test Report.  
- Ví dụ: Báo cáo nêu lỗi hiệu suất và đề xuất tối ưu API.  
**Nộp bài**: File markdown hoặc Word chứa Test Report.  

---

#### Hướng Dẫn Nộp Bài
- **Định dạng**: File markdown hoặc Word, đặt tên theo mẫu: `[Họ_Tên]_Manual_Testing_Assignment.md`.  
- **Thời hạn**: 1 tuần sau buổi học.  
- **Đánh giá**:  
  - Tính đầy đủ: Bao phủ yêu cầu bài tập.  
  - Tính chính xác: Nội dung đúng theo mẫu slide.  
  - Tính sáng tạo: Ví dụ thực tế, giải pháp đề xuất.  

