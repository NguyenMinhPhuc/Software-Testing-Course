# Hướng Dẫn Trưởng Nhóm: Quản Lý Tiến Độ và Phân Công Báo Cáo Cuối Kỳ

## Giới Thiệu
Tài liệu này cung cấp hướng dẫn chi tiết cho **trưởng nhóm** của các nhóm sinh viên (4-5 thành viên) thực hiện báo cáo cuối kỳ học phần **Kiểm Thử Phần Mềm**, theo quy định trong `Final_Report_Guidelines_Software_Testing.md`. Trưởng nhóm chịu trách nhiệm điều phối công việc, phân công vai trò, quản lý tiến độ, và đảm bảo chất lượng đầu ra (báo cáo viết và thuyết trình) trong 3 tuần.

- **Dự án**: Todo App (web) – kiểm thử thủ công các tính năng tạo, xóa, lọc công việc, và tương thích trình duyệt.
- **Nhiệm vụ**: Lập Test Plan, viết Test Case, thực thi kiểm thử, lập Test Report, chuẩn bị thuyết trình.
- **Thời gian**: 3 tuần (từ công bố đến hạn nộp).
- **Kết quả**: Báo cáo viết (PDF, 10-15 trang), slide thuyết trình (PPTX, 10-12 slide).

## Vai Trò và Trách Nhiệm Trưởng Nhóm
- **Điều phối**: Lập kế hoạch, tổ chức họp, theo dõi tiến độ.  
- **Phân công**: Gán vai trò và nhiệm vụ cho thành viên, đảm bảo công bằng.  
- **Giám sát**: Kiểm tra chất lượng công việc, đảm bảo đúng hạn và yêu cầu.  
- **Tổng hợp**: Hợp nhất các phần (Test Plan, Test Case, Test Report) thành báo cáo hoàn chỉnh.  
- **Liên lạc**: Đại diện nhóm giao tiếp với giảng viên, báo cáo vấn đề (nếu có).  
- **Thuyết trình**: Điều hành phần trình bày, đảm bảo tất cả thành viên tham gia.

## Hướng Dẫn Quản Lý Tiến Độ

### Tuần 1: Lập Kế Hoạch và Bắt Đầu
**Mục tiêu**: Phân tích PRD, lập Test Plan, bắt đầu viết Test Case.  
**Thời gian**: 7 ngày.  
**Các bước**:
1. **Tổ chức họp nhóm lần 1 (ngày 1-2)**:  
   - **Mục đích**: Thống nhất kế hoạch, phân vai trò, thảo luận PRD Todo App.  
   - **Hoạt động**:  
     - Giới thiệu quy định báo cáo (tham khảo `Final_Report_Guidelines_Software_Testing.md`).  
     - Phân tích PRD giả định (tính năng: tạo, xóa, lọc công việc; yêu cầu phi chức năng).  
     - Phân vai trò (xem phần "Phân Công Công Việc" dưới đây).  
   - **Kết quả**: Biên bản họp (mô tả vai trò, kế hoạch sơ bộ), lưu trong phụ lục báo cáo.  
   - **Công cụ**: Google Docs, Zoom, hoặc bảng trắng.  
2. **Lập kế hoạch chi tiết (ngày 2)**:  
   - Chia nhỏ nhiệm vụ theo tuần:  
     - Tuần 1: Test Plan (2-3 ngày), Test Case (4-5 ngày).  
     - Tuần 2: Thực thi kiểm thử (3-4 ngày), Test Report (3-4 ngày).  
     - Tuần 3: Hoàn thiện báo cáo (3-4 ngày), thuyết trình (3-4 ngày).  
   - Xác định mốc thời gian:  
     - Hạn nội bộ: Test Plan (ngày 5), Test Case (ngày 7).  
     - Họp kiểm tra: Ngày 4 và ngày 7.  
   - **Kết quả**: Lịch trình công việc (bảng hoặc biểu đồ Gantt), chia sẻ với nhóm.  
3. **Theo dõi tiến độ (ngày 3-7)**:  
   - **Test Plan**: Kiểm tra bản nháp (ngày 4), hoàn thiện (ngày 5).  
   - **Test Case**: Theo dõi số lượng Test Case (mục tiêu: 8-10 Test Case vào ngày 7).  
   - **Công cụ theo dõi**: Trello, Excel, hoặc Google Sheets (cột: Nhiệm vụ, Người phụ trách, Trạng thái, Hạn chót).  
   - **Hành động**: Nhắc nhở thành viên, hỗ trợ giải quyết khó khăn (ví dụ: làm rõ PRD).  
4. **Họp nhóm lần 2 (ngày 7)**:  
   - **Mục đích**: Đánh giá Test Plan, duyệt Test Case, lên kế hoạch tuần 2.  
   - **Hoạt động**:  
     - Xem xét Test Plan (đầy đủ phạm vi, tiêu chí, rủi ro?).  
     - Kiểm tra Test Case (bao phủ TR, trường hợp đa dạng?).  
     - Phân công nhiệm vụ tuần 2 (thực thi, Test Report).  
   - **Kết quả**: Biên bản họp, Test Plan hoàn chỉnh, ít nhất 10 Test Case.

### Tuần 2: Thực Thi và Báo Cáo
**Mục tiêu**: Hoàn thành Test Case, thực thi kiểm thử, lập Test Report.  
**Thời gian**: 7 ngày.  
**Các bước**:
1. **Hoàn thiện Test Case (ngày 8-9)**:  
   - Đảm bảo đủ 15 Test Case, bao phủ các trường hợp bình thường, lỗi, biên.  
   - Trưởng nhóm kiểm tra: Liên kết với TR, định dạng đúng (ID, bước, kết quả mong đợi).  
   - **Hành động**: Yêu cầu chỉnh sửa nếu Test Case thiếu sót (ví dụ: thêm trường hợp biên).  
2. **Thực thi kiểm thử (ngày 10-13)**:  
   - **Mô phỏng kiểm thử**: Giả định kết quả Pass/Fail, phát hiện ít nhất 3 lỗi (1 nghiêm trọng, 2 không nghiêm trọng).  
   - **Theo dõi**: Ghi kết quả vào bảng (Excel/Google Sheets), bao gồm:  
     - Test Case ID, Kết quả (Pass/Fail), Lỗi (nếu có).  
     - Lỗi: ID, mô tả, mức độ, trạng thái.  
   - **Hành động**: Kiểm tra tính nhất quán của kết quả, đảm bảo lỗi có mô tả chi tiết.  
3. **Lập Test Report (ngày 12-14)**:  
   - **Bản nháp**: Ngày 12 (tóm tắt kết quả, lỗi, ma trận truy xuất).  
   - **Hoàn thiện**: Ngày 14 (thêm đánh giá, khuyến nghị).  
   - **Hành động**: Trưởng nhóm duyệt bản nháp, đảm bảo đúng mẫu (Slide 2, 3, Lecture_5).  
4. **Họp nhóm lần 3 (ngày 14)**:  
   - **Mục đích**: Đánh giá kết quả kiểm thử, duyệt Test Report, lên kế hoạch tuần 3.  
   - **Hoạt động**:  
     - Xem xét kết quả kiểm thử (tỷ lệ Pass/Fail, lỗi phát hiện).  
     - Kiểm tra Test Report (đầy đủ, khuyến nghị cụ thể?).  
     - Phân công: Soạn báo cáo, chuẩn bị thuyết trình.  
   - **Kết quả**: Biên bản họp, Test Report hoàn chỉnh, kế hoạch tuần 3.

### Tuần 3: Hoàn Thiện và Thuyết Trình
**Mục tiêu**: Hoàn thiện báo cáo, chuẩn bị và tập dượt thuyết trình.  
**Thời gian**: 7 ngày.  
**Các bước**:
1. **Hợp nhất báo cáo (ngày 15-18)**:  
   - **Cấu trúc**: Theo quy định (trang bìa, mục lục, các phần 1-6, phụ lục).  
   - **Hành động**:  
     - Trưởng nhóm phân công:  
       - 1-2 thành viên hợp nhất Test Plan, Test Case, Test Report.  
       - 1 thành viên viết phần giới thiệu, kết luận.  
       - 1 thành viên định dạng (font, mục lục, trang bìa).  
     - Kiểm tra: Đúng định dạng (Times New Roman, 12, 10-15 trang), không sai chính tả.  
   - **Kết quả**: Bản nháp báo cáo (ngày 17), bản cuối (ngày 18, PDF).  
2. **Chuẩn bị thuyết trình (ngày 16-19)**:  
   - **Slide PowerPoint**: 10-12 slide (giới thiệu, Test Plan, Test Case, kết quả, Test Report, khuyến nghị).  
   - **Phân công**:  
     - 1-2 thành viên thiết kế slide (sử dụng template đơn giản, font Arial/Calibri).  
     - Mỗi thành viên chuẩn bị phần trình bày (2-3 phút).  
   - **Hành động**: Trưởng nhóm duyệt slide (ngày 18), tổ chức tập dượt (ngày 19).  
3. **Tập dượt thuyết trình (ngày 19-20)**:  
   - **Mục đích**: Đảm bảo trình bày trôi chảy, đúng thời lượng (10-15 phút).  
   - **Hoạt động**:  
     - Mỗi thành viên trình bày phần của mình.  
     - Trưởng nhóm ghi chú: Giọng nói, tốc độ, phối hợp giữa các phần.  
   - **Kết quả**: Slide PowerPoint hoàn chỉnh, nhóm sẵn sàng thuyết trình.  
4. **Nộp bài và thuyết trình (ngày 21)**:  
   - **Nộp bài**:  
     - File PDF: `[Tên_Nhóm]_Final_Report_Software_Testing.pdf`.  
     - File PPTX: `[Tên_Nhóm]_Final_Presentation.pptx`.  
     - Nộp qua LMS hoặc email trước 23:59.  
   - **Thuyết trình**: Theo lịch giảng viên, trưởng nhóm điều phối, đảm bảo tất cả thành viên tham gia.

## Phân Công Công Việc
Trưởng nhóm phân công vai trò và nhiệm vụ dựa trên kỹ năng và sở thích của thành viên, nhưng đảm bảo mỗi người tham gia ít nhất 2 nhiệm vụ chính. Gợi ý phân công:

| Vai trò                     | Nhiệm vụ chính                                                                 | Số thành viên |
|-----------------------------|-------------------------------------------------------------------------------|---------------|
| **Trưởng nhóm**             | - Điều phối, theo dõi tiến độ, tổng hợp báo cáo, dẫn dắt thuyết trình.        | 1             |
| **Người lập Test Plan**     | - Phân tích PRD, viết Test Plan, xác định rủi ro.                            | 1-2           |
| **Người viết Test Case**    | - Thiết kế 15 Test Case, đảm bảo bao phủ TR và trường hợp đa dạng.           | 2             |
| **Người thực thi kiểm thử** | - Mô phỏng kiểm thử, ghi kết quả Pass/Fail, mô tả lỗi (3 lỗi giả định).      | 1-2           |
| **Người lập Test Report**   | - Tổng hợp kết quả, viết Test Report, đưa ra khuyến nghị.                    | 1-2           |
| **Người chuẩn bị thuyết trình** | - Thiết kế slide, tập dượt, trình bày phần của mình.                      | Tất cả        |

**Lưu ý**:
- **Công bằng**: Mỗi thành viên tham gia ít nhất 2 nhiệm vụ (ví dụ: viết Test Case + thuyết trình).  
- **Ghi nhận đóng góp**: Trưởng nhóm ghi lại đóng góp của từng thành viên trong biên bản họp, báo cáo giảng viên nếu có thành viên không tham gia.  
- **Linh hoạt**: Điều chỉnh vai trò nếu thành viên gặp khó khăn (ví dụ: hỗ trợ thêm cho Test Case nếu chậm tiến độ).

## Mẹo Quản Lý Hiệu Quả
1. **Giao tiếp thường xuyên**:  
   - Tạo nhóm chat (Zalo, Telegram) để cập nhật tiến độ hàng ngày.  
   - Đặt quy tắc: Phản hồi trong 24 giờ, báo cáo vấn đề ngay.  
2. **Sử dụng công cụ**:  
   - **Trello**: Quản lý nhiệm vụ (bảng: To Do, Doing, Done).  
   - **Google Docs/Sheets**: Soạn thảo, theo dõi Test Case, kết quả kiểm thử.  
   - **Canva/PowerPoint**: Thiết kế slide thuyết trình.  
3. **Giải quyết xung đột**:  
   - Nếu thành viên chậm tiến độ: Gặp riêng, hỗ trợ hoặc điều chỉnh nhiệm vụ.  
   - Nếu bất đồng ý kiến: Tổ chức bỏ phiếu hoặc xin ý kiến giảng viên.  
4. **Kiểm tra chất lượng**:  
   - Duyệt từng phần (Test Plan, Test Case, Test Report) trước khi hợp nhất.  
   - Sử dụng checklist: Đầy đủ nội dung, đúng định dạng, không sai chính tả.  
5. **Khuyến khích nhóm**:  
   - Ghi nhận đóng góp (ví dụ: cảm ơn thành viên hoàn thành sớm).  
   - Tạo không khí tích cực: Họp ngắn gọn, tập trung, có thời gian thư giãn.

## Xử Lý Vấn Đề
- **Chậm tiến độ**:  
  - Xác định nguyên nhân (nhiệm vụ khó, thiếu nguồn lực?).  
  - Phân công lại hoặc hỗ trợ (ví dụ: trưởng nhóm giúp viết Test Case).  
  - Báo cáo giảng viên nếu cần gia hạn (trước hạn 2 ngày).  
- **Thành viên không tham gia**:  
  - Gửi cảnh báo qua nhóm chat, ghi nhận trong biên bản họp.  
  - Báo cáo giảng viên (kèm bằng chứng: biên bản, tin nhắn) để trừ điểm cá nhân.  
- **Khó khăn kỹ thuật**:  
  - Tham khảo slide bài giảng (Lecture_2, Lecture_4, Lecture_5) hoặc bài giải mẫu (`Sample_Solution_Manual_Testing_TodoApp.md`).  
  - Liên hệ giảng viên qua email/diễn đàn để được hướng dẫn.

## Kết Quả Mong Đợi
- **Báo cáo viết**: PDF chuyên nghiệp, đầy đủ 6 phần, đúng định dạng, 10-15 trang.  
- **Thuyết trình**: Slide rõ ràng, trình bày trôi chảy, tất cả thành viên tham gia.  
- **Tiến độ**: Hoàn thành đúng hạn, không trễ nộp.  
- **Nhóm**: Phân công công bằng, phối hợp nhịp nhàng, biên bản họp đầy đủ.

## Tài Liệu Tham Khảo
- **Quy định báo cáo**: `Final_Report_Guidelines_Software_Testing.md`.  
- **Slide bài giảng**:  
  - Lecture_2_Building_Test_Plan.md (Slide 2, 3, 5-7).  
  - Lecture_4_Test_Case_Design.md (Slide 2, 3, 6-8).  
  - Lecture_5_Test_Report.md (Slide 2, 3, 6-8).  
- **Bài giải mẫu**: `Sample_Solution_Manual_Testing_TodoApp.md` (Trong thư mục Example trên github).