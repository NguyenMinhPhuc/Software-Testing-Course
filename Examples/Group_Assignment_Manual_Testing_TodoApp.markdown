# Bài Tập Nhóm: Thực Hành Kiểm Thử Thủ Công Trên Todo App

## Thông Tin Chung
- **Mục tiêu**: Áp dụng kiến thức kiểm thử thủ công để lập kế hoạch, thiết kế, thực thi, và báo cáo kiểm thử cho ứng dụng Todo App.
- **Số lượng thành viên**: 4-5 sinh viên mỗi nhóm.
- **Thời gian thực hiện**: 2-3 giờ (bao gồm thảo luận, thực hành, và nộp bài).
- **Ứng dụng**: Todo App (web) – một ứng dụng quản lý công việc cho phép người dùng:
  - Tạo, chỉnh sửa, xóa công việc.
  - Gắn thẻ ưu tiên (Cao, Trung, Thấp).
  - Lọc công việc theo trạng thái (Hoàn thành, Chưa hoàn thành) hoặc ưu tiên.
  - Tương thích với trình duyệt Chrome và Firefox.
- **PRD giả định**: Todo App có các tính năng chính như trên, với yêu cầu hiệu suất (lọc công việc < 1 giây) và tương thích giao diện trên các trình duyệt.

## Mục Tiêu Học Tập
- Hiểu và áp dụng quy trình kiểm thử thủ công (lập Test Plan, viết Test Case, thực thi, lập Test Report).
- Phân chia công việc nhóm hiệu quả, phối hợp giữa các thành viên.
- Phát triển kỹ năng phân tích yêu cầu, thiết kế kiểm thử, và báo cáo lỗi.

## Vai Trò Trong Nhóm
- **Trưởng nhóm**: Điều phối công việc, đảm bảo tiến độ, tổng hợp bài nộp.
- **Người lập Test Plan**: Phân tích PRD, soạn Test Plan.
- **Người viết Test Case**: Thiết kế Test Case dựa trên yêu cầu.
- **Người thực thi kiểm thử**: Thực hiện Test Case, ghi lại kết quả.
- **Người lập Test Report**: Tổng hợp kết quả, viết báo cáo kiểm thử.
- **Lưu ý**: Các thành viên có thể đảm nhận nhiều vai trò, nhưng mỗi nhiệm vụ cần được phân công rõ ràng.

## Nhiệm Vụ Nhóm

### Nhiệm Vụ 1: Lập Test Plan
**Mô tả**:  
- Nhóm phân tích PRD giả định của Todo App để lập Test Plan cơ bản, xác định chiến lược kiểm thử thủ công.  
**Yêu cầu**:  
- Test Plan bao gồm:  
  - **Phạm vi**: Tính năng kiểm thử (tạo, xóa, lọc công việc); ngoài phạm vi (ví dụ: tích hợp Google Calendar).  
  - **Mục tiêu chất lượng**: 90% test case passed, không có lỗi nghiêm trọng.  
  - **Phương pháp**: Kiểm thử thủ công hộp đen, theo Agile.  
  - **Tài nguyên**: Công cụ quản lý (TestRail hoặc Excel), môi trường (Chrome, Firefox trên Windows 10).  
  - **Tiêu chí hoàn thành**: 90% bao phủ yêu cầu, lỗi nghiêm trọng được sửa.  
- Sử dụng mẫu từ Slide 2, 3 (Lecture_2_Building_Test_Plan).  
**Hướng dẫn**:  
- Tham khảo Slide 5-7 (Lecture_2) về Test Plan của Todo App.  
- Ví dụ: Phạm vi bao gồm kiểm thử tạo công việc, tiêu chí hoàn thành là 90% test case passed.  
**Kết quả**: File markdown hoặc Word chứa Test Plan (1-2 trang).

---

### Nhiệm Vụ 2: Viết Test Case
**Mô tả**:  
- Nhóm thiết kế 10 Test Case chi tiết cho các tính năng **tạo công việc**, **xóa công việc**, và **lọc công việc** của Todo App.  
**Yêu cầu kiểm thử (TR)**:  
- TR-001: Tạo công việc với tiêu đề tối đa 200 ký tự.  
- TR-002: Xóa công việc, yêu cầu xác nhận trước khi xóa.  
- TR-003: Lọc công việc theo trạng thái "Hoàn thành" hoặc "Chưa hoàn thành".  
- TR-004: Tương thích giao diện trên Chrome và Firefox.  
**Yêu cầu**:  
- Mỗi Test Case bao gồm:  
  - ID (TC-001, TC-002, ...).  
  - Mô tả (mục tiêu kiểm thử).  
  - Điều kiện tiên quyết (ứng dụng chạy trên Chrome).  
  - Bước thực hiện (các bước cụ thể).  
  - Kết quả mong đợi (ví dụ: công việc hiển thị trong danh sách).  
- Bao phủ:  
  - Trường hợp bình thường (ví dụ: tạo công việc hợp lệ).  
  - Trường hợp lỗi (ví dụ: tiêu đề rỗng).  
  - Trường hợp biên (ví dụ: tiêu đề 200 ký tự).  
- Sử dụng mẫu từ Slide 2, 3 (Lecture_4_Test_Case_Design).  
**Hướng dẫn**:  
- Tham khảo Slide 6-8 (Lecture_4) về Test Case của Todo App.  
- Ví dụ: TC-001 kiểm tra tạo công việc với tiêu đề "Họp nhóm", kết quả hiển thị đúng.  
**Kết quả**: File markdown hoặc Word chứa 10 Test Case.

---

### Nhiệm Vụ 3: Thực Thi Kiểm Thử
**Mô tả**:  
- Nhóm giả định thực thi 10 Test Case từ Nhiệm Vụ 2 trên Todo App (sử dụng môi trường mô phỏng hoặc kịch bản giả định).  
- Ghi lại kết quả (Pass/Fail) và phát hiện lỗi (nếu có).  
**Yêu cầu**:  
- Mô phỏng kết quả kiểm thử với ít nhất 2 lỗi giả định:  
  - 1 lỗi nghiêm trọng (ví dụ: lọc công việc chậm với 1,000 công việc).  
  - 1 lỗi không nghiêm trọng (ví dụ: giao diện lệch trên Firefox).  
- Ghi lại:  
  - Kết quả thực tế (Pass/Fail) cho mỗi Test Case.  
  - Mô tả lỗi (ID, mức độ, trạng thái: chưa sửa/đã sửa).  
**Hướng dẫn**:  
- Tham khảo Slide 3 (Lecture_5_Test_Report) về thu thập kết quả kiểm thử.  
- Ví dụ: TC-003 (lọc công việc) failed do thời gian lọc > 1 giây.  
**Kết quả**: File markdown hoặc Word chứa bảng kết quả kiểm thử và danh sách lỗi.

---

### Nhiệm Vụ 4: Lập Test Report
**Mô tả**:  
- Nhóm tổng hợp kết quả từ Nhiệm Vụ 3 để lập Test Report, đánh giá chất lượng Todo App và đưa ra khuyến nghị.  
**Yêu cầu**:  
- Test Report bao gồm:  
  - **Thông tin chung**: Tên dự án (Todo App), phiên bản (1.0), ngày kiểm thử (giả định: 01/06/2025).  
  - **Tóm tắt kết quả**: Số Test Case, tỷ lệ Pass/Fail (ví dụ: 8/10 passed), tỷ lệ bao phủ yêu cầu.  
  - **Phân tích lỗi**: Danh sách lỗi (ID, mô tả, mức độ, trạng thái).  
  - **Ma trận truy xuất**: Liên kết Test Case với TR (ví dụ: TC-001 liên quan TR-001).  
  - **Đánh giá và khuyến nghị**: Chất lượng ứng dụng, hành động tiếp theo (sửa lỗi, kiểm thử lại).  
- Sử dụng mẫu từ Slide 2, 3 (Lecture_5_Test_Report).  
**Hướng dẫn**:  
- Tham khảo Slide 6-8 (Lecture_5) về Test Report của Todo App.  
- Ví dụ: Báo cáo đề xuất sửa lỗi hiệu suất lọc công việc trước phát hành.  
**Kết quả**: File markdown hoặc Word chứa Test Report (1-2 trang).

---

## Hướng Dẫn Thực Hiện
1. **Phân công vai trò**:  
   - Trưởng nhóm phân chia nhiệm vụ (lập Test Plan, viết Test Case, thực thi, lập Test Report).  
   - Mỗi thành viên tham gia ít nhất 1 nhiệm vụ, nhưng có thể hỗ trợ lẫn nhau.  
2. **Thảo luận nhóm**:  
   - Dành 30 phút đầu để phân tích PRD giả định và thống nhất cách tiếp cận.  
   - Sử dụng bảng trắng hoặc công cụ trực tuyến (Miro, Google Docs) để ghi ý tưởng.  
3. **Thực hiện nhiệm vụ**:  
   - Nhiệm Vụ 1 (Test Plan): 30 phút.  
   - Nhiệm Vụ 2 (Test Case): 45 phút.  
   - Nhiệm Vụ 3 (Thực thi): 30 phút.  
   - Nhiệm Vụ 4 (Test Report): 45 phút.  
4. **Tổng hợp và nộp bài**:  
   - Trưởng nhóm kiểm tra và hợp nhất các kết quả vào một file duy nhất.  
   - Đảm bảo định dạng rõ ràng, có tiêu đề cho từng nhiệm vụ.

## Hướng Dẫn Nộp Bài
- **Định dạng**: File markdown hoặc Word, đặt tên theo mẫu: `[Tên_Nhóm]_Manual_Testing_Group_Assignment.md`.  
- **Nội dung**: Bao gồm:  
  - Danh sách thành viên và vai trò.  
  - Kết quả của 4 nhiệm vụ (Test Plan, Test Case, Kết quả kiểm thử, Test Report).  
- **Thời hạn**: 1 tuần sau buổi thực hành.  
- **Nộp qua**: Email hoặc hệ thống quản lý học tập (LMS).  

## Tiêu Chí Đánh Giá
- **Tính đầy đủ (30%)**: Hoàn thành tất cả 4 nhiệm vụ, bao phủ yêu cầu.  
- **Tính chính xác (30%)**: Nội dung đúng theo mẫu từ các slide (Test Plan, Test Case, Test Report).  
- **Tính sáng tạo (20%)**: Ví dụ thực tế, giải pháp đề xuất, khuyến nghị trong Test Report.  
- **Làm việc nhóm (20%)**: Phân công rõ ràng, kết quả đồng nhất, trình bày chuyên nghiệp.  

## Tài Liệu Tham Khảo
- **Slide bài giảng**:  
  - Lecture_2_Building_Test_Plan.md (Slide 2, 3, 5-7).  
  - Lecture_4_Test_Case_Design.md (Slide 2, 3, 6-8).  
  - Lecture_5_Test_Report.md (Slide 2, 3, 6-8).  
- **Công cụ gợi ý**:  
  - Excel/Google Sheets để viết Test Case.  
  - TestRail (mô phỏng) để quản lý Test Case và kết quả.  
  - Google Docs để soạn Test Plan và Test Report.  

## Ví Dụ Kết Quả
- **Test Plan (trích đoạn)**:  
  - **Phạm vi**: Kiểm thử tạo, xóa, lọc công việc; ngoài phạm vi là tích hợp Google Calendar.  
  - **Tiêu chí hoàn thành**: 90% Test Case passed, lỗi nghiêm trọng được sửa.  
- **Test Case (trích đoạn)**:  
  - **TC-001**:  
    - **Mô tả**: Kiểm tra tạo công việc với tiêu đề hợp lệ.  
    - **Bước thực hiện**: 1. Mở Todo App. 2. Nhập tiêu đề "Họp nhóm". 3. Nhấn "Thêm".  
    - **Kết quả mong đợi**: Công việc hiển thị trong danh sách.  
- **Test Report (trích đoạn)**:  
  - **Tóm tắt**: 10 Test Case, 8 passed (80%), 90% bao phủ yêu cầu.  
  - **Lỗi**: BUG-001 (Hiệu suất lọc chậm, mức cao, chưa sửa).  
  - **Khuyến nghị**: Tối ưu API lọc, kiểm thử lại với 1,000 công việc.