# Quy Định Làm Báo Cáo Cuối Kỳ - Học Phần Kiểm Thử Phần Mềm

## Thông Tin Chung
- **Học phần**: Kiểm Thử Phần Mềm.  
- **Hình thức**: Làm việc nhóm (4-5 sinh viên/nhóm).  
- **Mục tiêu**:  
  - Áp dụng kiến thức kiểm thử thủ công (Test manual) (từ các bài giảng) vào một dự án do nhóm lựa chọn.  
  - Phát triển kỹ năng lập kế hoạch kiểm thử, thiết kế Test Case, thực thi kiểm thử, báo cáo, và làm việc nhóm.  
  - Trình bày kết quả kiểm thử một cách chuyên nghiệp.  
- **Thời gian thực hiện**: 3 tuần (từ khi công bố đến hạn nộp).  
- **Hình thức nộp**: Báo cáo viết (file PDF) và thuyết trình (PowerPoint, 10-15 phút/nhóm).  
- **Trọng số điểm**: Báo cáo chiếm 40% điểm học phần (30% báo cáo viết, 10% thuyết trình).

## Yêu Cầu Báo Cáo Cuối Kỳ

### 1. Bối Cảnh Dự Án
- **Ứng dụng**: nhóm tự động chọn một phần mềm có sắn trên hệ điều hành Windows  để tiến hành kiểm thử theo yêu cầu 
- **ví dụ**:
  - Ứng dụng: Todo App (web) – cho phép người dùng:  
  - Tạo, chỉnh sửa, xóa công việc.  
  - Gắn thẻ ưu tiên (Cao, Trung, Thấp).  
  - Lọc công việc theo trạng thái (Hoàn thành, Chưa hoàn thành) hoặc ưu tiên.  
  - Yêu cầu phi chức năng: Hiệu suất lọc < 1 giây, tương thích Chrome/Firefox.  
- **PRD giả định**: Cung cấp danh sách tính năng và yêu cầu (tham khảo Lecture_3_Test_Requirements.md).  
- **Môi trường kiểm thử**: Windows 10, Chrome (phiên bản mới nhất), Firefox (phiên bản mới nhất).

### 2. Nhiệm Vụ Nhóm
Nhóm thực hiện một quy trình kiểm thử thủ công hoàn chỉnh cho Ứng dụng nhóm đã chọn (Todo App), bao gồm:

#### Nhiệm Vụ 1: Lập Test Plan
- **Mô tả**: Xây dựng Test Plan chi tiết, xác định chiến lược kiểm thử thủ công.  
- **Yêu cầu**:  
  - Bao gồm:  
    - Phạm vi (trong/ngoài phạm vi).  
    - Mục tiêu chất lượng (ví dụ: 90% Test Case passed).  
    - Phương pháp kiểm thử (thủ công, hộp đen, Agile).  
    - Tài nguyên (công cụ: Excel/Jira, môi trường: Chrome/Firefox).  
    - Tiêu chí hoàn thành (ví dụ: 95% bao phủ yêu cầu).  
    - Rủi ro và kế hoạch giảm thiểu.  
  - Tham khảo mẫu: Slide 2, 3, 5-7 (Lecture_2_Building_Test_Plan.md).  
- **Kết quả**: Phần Test Plan trong báo cáo (2-3 trang).

#### Nhiệm Vụ 2: Thiết Kế Test Case
- **Mô tả**: Viết ít nhất 15 Test Case cho các tính năng chính (tạo, xóa, lọc công việc, tương thích trình duyệt).  
- **Yêu cầu**:  
  - Bao gồm: ID, mô tả, điều kiện tiên quyết, bước thực hiện, kết quả mong đợi.  
  - Bao phủ:  
    - Trường hợp bình thường (ví dụ: tạo công việc hợp lệ).  
    - Trường hợp lỗi (ví dụ: tiêu đề rỗng).  
    - Trường hợp biên (ví dụ: tiêu đề 200 ký tự).  
  - Liên kết với yêu cầu kiểm thử (TR) từ PRD.  
  - Tham khảo mẫu: Slide 2, 3, 6-8 (Lecture_4_Test_Case_Design.md).  
- **Kết quả**: Phần Test Case trong báo cáo (bảng, 3-4 trang).

#### Nhiệm Vụ 3: Thực Thi Kiểm Thử
- **Mô tả**: Giả định thực thi Test Case trên Todo App (môi trường mô phỏng), ghi lại kết quả và lỗi.  
- **Yêu cầu**:  
  - Báo cáo kết quả: Pass/Fail cho mỗi Test Case.  
  - Phát hiện ít nhất 3 lỗi giả định:  
    - 1 lỗi nghiêm trọng (Critical/High, ví dụ: hiệu suất lọc chậm).  
    - 2 lỗi không nghiêm trọng (Medium/Low, ví dụ: giao diện lệch).  
  - Mô tả lỗi: ID, mức độ, trạng thái (chưa sửa/đã sửa), Test Case liên quan.  
  - Tham khảo mẫu: Slide 3 (Lecture_5_Test_Report.md).  
- **Kết quả**: Phần kết quả kiểm thử và lỗi trong báo cáo (bảng, 1-2 trang).

#### Nhiệm Vụ 4: Lập Test Report
- **Mô tả**: Tổng hợp kết quả kiểm thử, đánh giá chất lượng Todo App, và đưa ra khuyến nghị.  
- **Yêu cầu**:  
  - Bao gồm:  
    - Thông tin chung (dự án, phiên bản, ngày kiểm thử).  
    - Tóm tắt kết quả (số Test Case, tỷ lệ Pass/Fail, bao phủ yêu cầu).  
    - Phân tích lỗi (ID, mô tả, mức độ, trạng thái).  
    - Ma trận truy xuất (liên kết TR với Test Case).  
    - Đánh giá và khuyến nghị (chất lượng, hành động tiếp theo).  
  - Tham khảo mẫu: Slide 2, 3, 6-8 (Lecture_5_Test_Report.md).  
- **Kết quả**: Phần Test Report trong báo cáo (2-3 trang).

#### Nhiệm Vụ 5: Thuyết Trình
- **Mô tả**: Chuẩn bị bài thuyết trình tóm tắt quy trình kiểm thử và kết quả.  
- **Yêu cầu**:  
  - Slide PowerPoint (10-12 slide):  
    - Giới thiệu dự án Todo App.  
    - Tóm tắt Test Plan, Test Case, kết quả kiểm thử, Test Report.  
    - Khuyến nghị và bài học kinh nghiệm.  
  - Thời lượng: 10-15 phút (bao gồm Q&A).  
  - Tất cả thành viên phải tham gia thuyết trình.  
- **Kết quả**: File PowerPoint (.pptx) nộp cùng báo cáo.

### 3. Cấu Trúc Báo Cáo Viết
- **Trang bìa**: Tên học phần, tên nhóm, danh sách thành viên, ngày nộp.  
- **Mục lục**: Liệt kê các phần và số trang.  
- **Phần 1**: Giới thiệu (mô tả Todo App, mục tiêu báo cáo, vai trò thành viên).  
- **Phần 2**: Test Plan (theo Nhiệm Vụ 1).  
- **Phần 3**: Test Case (theo Nhiệm Vụ 2).  
- **Phần 4**: Kết quả kiểm thử và lỗi (theo Nhiệm Vụ 3).  
- **Phần 5**: Test Report (theo Nhiệm Vụ 4).  
- **Phần 6**: Kết luận và bài học kinh nghiệm (1 trang).  
- **Tài liệu tham khảo**: Trích dẫn slide bài giảng hoặc nguồn khác (nếu có).  
- **Phụ lục** (nếu cần): Biểu đồ, ảnh chụp màn hình, tài liệu bổ sung.  
- **Định dạng**:  
  - Font: Times New Roman, size 12.  
  - Độ dài: 10-15 trang (không tính trang bìa, mục lục, phụ lục).  
  - File PDF, đặt tên: `[Tên_Nhóm]_Final_Report_Software_Testing.pdf`.

### 4. Quy Trình Thực Hiện
1. **Thành lập nhóm**:  
   - Tự chọn hoặc giảng viên chỉ định (4-5 thành viên).  
   - Phân vai trò: Trưởng nhóm, người lập Test Plan, viết Test Case, thực thi, báo cáo, thuyết trình.  
2. **Lập kế hoạch**:  
   - Tuần 1: Phân tích PRD, lập Test Plan, viết Test Case.  
   - Tuần 2: Thực thi kiểm thử (mô phỏng), lập Test Report.  
   - Tuần 3: Hoàn thiện báo cáo, chuẩn bị thuyết trình.  
3. **Họp nhóm**:  
   - Họp ít nhất 3 lần (ghi biên bản họp, nộp trong phụ lục).  
   - Sử dụng công cụ hỗ trợ: Google Docs, Miro, hoặc Excel.  
4. **Nộp bài**:  
   - Nộp báo cáo (PDF) và slide thuyết trình (PPTX) qua hệ thống LMS hoặc email.  
   - Hạn nộp: 23:59, ngày cuối tuần thứ 3.  
   - Trễ hạn: Trừ 10% điểm/ngày.  
5. **Thuyết trình**:  
   - Tổ chức trong tuần cuối kỳ (lịch do giảng viên cung cấp).  
   - Mỗi thành viên trình bày ít nhất 2-3 phút.  

## Rubric Chấm Điểm

### 1. Báo Cáo Viết (30 điểm)
| Tiêu chí                     | Mô tả                                                                 | Điểm tối đa | 
|------------------------------|----------------------------------------------------------------------|-------------|
| **Nội dung (12 điểm)**       | - Test Plan đầy đủ, rõ ràng, phù hợp PRD (4 điểm).                   |             |
|                              | - Test Case bao phủ TR, đa dạng trường hợp (4 điểm).                 |             |
|                              | - Kết quả kiểm thử và Test Report chính xác, có khuyến nghị cụ thể (4 điểm). |             |
| **Tính chuyên nghiệp (8 điểm)** | - Cấu trúc báo cáo rõ ràng, đúng định dạng (4 điểm).                |             |
|                              | - Ngôn ngữ mạch lạc, không sai chính tả, ngữ pháp (4 điểm).          |             |
| **Sáng tạo (6 điểm)**        | - Đề xuất giải pháp sáng tạo (ví dụ: tối ưu kiểm thử, giảm rủi ro) (3 điểm). |             |
|                              | - Sử dụng biểu đồ, hình ảnh minh họa hiệu quả (3 điểm).              |             |
| **Làm việc nhóm (4 điểm)**   | - Phân công vai trò rõ ràng, biên bản họp đầy đủ (2 điểm).           |             |
|                              | - Đóng góp đồng đều giữa các thành viên (2 điểm).                    |             |

### 2. Thuyết Trình (10 điểm)
| Tiêu chí                     | Mô tả                                                                 | Điểm tối đa |
|------------------------------|----------------------------------------------------------------------|-------------|
| **Nội dung (4 điểm)**        | - Tóm tắt rõ ràng Test Plan, Test Case, kết quả, và khuyến nghị (2 điểm). |             |
|                              | - Trả lời câu hỏi chính xác, logic (2 điểm).                         |             |
| **Kỹ năng trình bày (4 điểm)** | - Giọng nói rõ ràng, tự tin, đúng thời lượng (2 điểm).              |             |
|                              | - Slide thiết kế chuyên nghiệp, dễ hiểu (2 điểm).                    |             |
| **Tham gia nhóm (2 điểm)**   | - Tất cả thành viên tham gia thuyết trình (1 điểm).                  |             |
|                              | - Phối hợp nhịp nhàng giữa các thành viên (1 điểm).                  |             |

### Tổng điểm
- Báo cáo viết: 30 điểm.  
- Thuyết trình: 10 điểm.  
- **Tổng**: 40 điểm (40% điểm học phần).  
- **Cách tính**: Điểm cuối = (Điểm báo cáo viết + Điểm thuyết trình) / 4 (thang 10).

## Lưu Ý
- **Đạo văn**: Báo cáo sao chép từ nhóm khác hoặc nguồn không trích dẫn sẽ bị 0 điểm.  
- **Đóng góp nhóm**: Thành viên không tham gia (dựa trên biên bản họp hoặc báo cáo trưởng nhóm) sẽ bị trừ 50% điểm cá nhân.  
- **Tài liệu tham khảo**:  
  - Lecture_2_Building_Test_Plan.md (Slide 2, 3, 5-7).  
  - Lecture_3_Test_Requirements.md (Slide 2, 5-7).  
  - Lecture_4_Test_Case_Design.md (Slide 2, 3, 6-8).  
  - Lecture_5_Test_Report.md (Slide 2, 3, 6-8).  
  - Bài giải mẫu: Sample_Solution_Manual_Testing_TodoApp.md (nếu có).  
- **Hỗ trợ**: Sinh viên có thể đặt câu hỏi qua email giảng viên (phuc@lhu.edu.vn)hoặc trực tiếp trên LMS.  

