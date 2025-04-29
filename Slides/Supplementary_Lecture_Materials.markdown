# Tài Liệu Bổ Sung Bài Giảng Kiểm Thử Thủ Công

## Phần 1: Slide Bổ Sung Cho Các File Bài Giảng

Dưới đây là các slide bổ sung (5 slide mỗi file) với ví dụ thực tế từ **ứng dụng quản lý công việc (Todo App)**, một ứng dụng web cho phép người dùng tạo, chỉnh sửa, xóa công việc, gắn thẻ ưu tiên, và lọc công việc theo trạng thái.

### 1.1 Bổ sung cho Lecture_1_Introduction_to_Software_Testing.md
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

### 1.2 Bổ sung cho Lecture_2_Building_Test_Plan.md
#### Slide 5: Ví Dụ Thực Tế - Test Plan Cho Todo App
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

#### Slide 6: Thành Phần Test Plan Trong Todo App
**Nội dung chính**:  
- **Phạm vi**: Tạo, chỉnh sửa, xóa công việc; tương thích trình duyệt.  
- **Mục tiêu chất lượng**: Không có lỗi nghiêm trọng, lọc công việc < 1 giây.  
- **Tài nguyên**: Công cụ TestRail, môi trường web (Chrome, Firefox).  
- **Tiêu chí hoàn thành**: 90% test case passed, lỗi cao được sửa.  
**Ví dụ**:  
- Todo App yêu cầu kiểm thử trên cấu hình tối thiểu (4GB RAM, Windows 10).  
**Hoạt động**: Liệt kê thành phần Test Plan cho Todo App.  

---

#### Slide 7: Quy Trình Lập Test Plan Cho Todo App
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

#### Slide 8: Rủi Ro Trong Test Plan Todo App
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

#### Slide 9: Linh Hoạt Trong Test Plan Todo App
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

---

### 1.3 Bổ sung cho Lecture_3_Test_Requirements.md
#### Slide 5: Ví Dụ Thực Tế - Yêu Cầu Kiểm Thử Todo App
**Nội dung chính**:  
- **Dự án**: Todo App.  
- **Yêu cầu kiểm thử**:  
  - **Chức năng**: Tạo/xóa công việc, lọc theo trạng thái.  
  - **Phi chức năng**: Hiệu suất lọc < 1 giây, tương thích Chrome/Firefox.  
**Ví dụ**:  
- TR-001: Người dùng có thể tạo công việc với tiêu đề tối đa 200 ký tự.  
**Hoạt động**: Thảo luận yêu cầu kiểm thử của Todo App so với Notepad Cải Tiến.  

---

#### Slide 6: Xác Định Yêu Cầu Trong Todo App
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

#### Slide 7: Tầm Quan Trọng Yêu Cầu Trong Todo App
**Nội dung chính**:  
- **Bao phủ**: Đảm bảo mọi tính năng (tạo, lọc, xóa) được kiểm thử.  
- **Hỗ trợ test case**: TR-001 dẫn đến test case kiểm tra nhập công việc.  
- **Giảm rủi ro**: Phát hiện thiếu sót (ví dụ: thiếu yêu cầu tương thích mobile).  
**Ví dụ**:  
- Todo App: TR-004 (Tương thích Firefox) giúp phát hiện lỗi giao diện.  
**Hoạt động**: Thảo luận hậu quả nếu bỏ sót yêu cầu trong Todo App.  

---

#### Slide 8: Thách Thức Yêu Cầu Trong Todo App
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

#### Slide 9: Xác Minh Yêu Cầu Trong Todo App
**Nội dung chính**:  
- **Quy trình xác minh**:  
  - Gửi danh sách yêu cầu cho khách hàng/đội phát triển.  
  - Sử dụng bảng câu hỏi (ví dụ: Giới hạn dữ liệu công việc?).  
- **Lợi ích**:  
  - Đảm bảo yêu cầu chính xác trước khi viết test case.  
**Ví dụ**:  
- Todo App: Xác minh TR-002 (lọc trạng thái) để bao gồm cả trạng thái rỗng.  
**Hoạt động**: Sinh viên đề xuất bảng câu hỏi xác minh yêu cầu cho Todo App.  

---

### 1.4 Bổ sung cho Lecture_4_Test_Case_Design.md
#### Slide 6: Ví Dụ Thực Tế - Test Case Cho Todo App
**Nội dung chính**:  
- **Dự án**: Todo App.  
- **Test Case**:  
  - Kiểm tra tạo công việc với tiêu đề hợp lệ.  
  - Kiểm tra lọc công việc theo trạng thái "hoàn thành".  
- **Cấu trúc**: ID, mô tả, bước thực hiện, kết quả mong đợi.  
**Ví dụ**:  
- TC-001: Tạo công việc, nhập tiêu đề "Họp nhóm", kết quả hiển thị trong danh sách.  
**Hoạt động**: Thảo luận test case của Todo App so với Notepad Cải Tiến.  

---

#### Slide 7: Xây Dựng Test Case Trong Todo App
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

#### Slide 8: Lưu Ý Test Case Trong Todo App
**Nội dung chính**:  
- **Đầy đủ**: Bao phủ tạo, xóa, lọc công việc.  
- **Rõ ràng**: Bước thực hiện dễ hiểu (nhấn nút "Thêm").  
- **Khả thi**: Kiểm tra trên Chrome/Firefox.  
**Ví dụ**:  
- TC-003: Lọc công việc "hoàn thành", kiểm tra trên Chrome, kết quả chính xác.  
**Hoạt động**: Thảo luận cách đảm bảo test case rõ ràng trong Todo App.  

---

#### Slide 9: Thách Thức Test Case Trong Todo App
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

#### Slide 10: Kiểm Tra Test Case Trong Todo App
**Nội dung chính**:  
- **Quy trình kiểm tra**:  
  - Đánh giá tính đầy đủ (bao phủ TR).  
  - Xác minh tính khả thi (môi trường kiểm thử).  
- **Lợi ích**:  
  - Đảm bảo test case thực thi hiệu quả, không dư thừa.  
**Ví dụ**:  
- Todo App: Kiểm tra TC-001 để đảm bảo bao phủ TR-001 (tạo công việc).  
**Hoạt động**: Sinh viên đánh giá một test case giả định cho Todo App.  

---

### 1.5 Bổ sung cho Lecture_5_Test_Report.md
#### Slide 6: Ví Dụ Thực Tế - Test Report Cho Todo App
**Nội dung chính**:  
- **Dự án**: Todo App.  
- **Test Report**:  
  - Tổng hợp kết quả kiểm thử tạo, xóa, lọc công việc.  
  - Báo cáo lỗi giao diện và hiệu suất.  
**Ví dụ**:  
- Test Report: 90% test case passed, 2 lỗi giao diện trên Firefox cần sửa.  
**Hoạt động**: Thảo luận Test Report của Todo App so với Notepad Cải Tiến.  

---

#### Slide 7: Thành Phần Test Report Trong Todo App
**Nội dung chính**:  
- **Thông tin chung**: Phiên bản 1.0, kiểm thử 01/06/2025.  
- **Tóm tắt**: 20 test case, 90% passed, 95% bao phủ.  
- **Lỗi**: 3 lỗi (1 cao, 2 thấp), 1 lỗi chưa sửa.  
- **Khuyến nghị**: Sửa lỗi trước phát hành.  
**Ví dụ**:  
- Todo App: Báo cáo nêu lỗi chậm khi lọc 1,000 công việc.  
**Hoạt động**: Liệt kê thành phần Test Report cho Todo App.  

---

#### Slide 8: Quy Trình Test Report Trong Todo App
**Nội dung chính**:  
- **Thu thập**: Kết quả test case từ TestRail.  
- **Tổng hợp lỗi**: Sử dụng Jira để theo dõi.  
- **Đánh giá**: Kiểm tra bao phủ qua ma trận truy xuất.  
- **Khuyến nghị**: Sửa lỗi hiệu suất và kiểm thử lại.  
**Ví dụ**:  
- Todo App: Báo cáo đề xuất tối ưu API lọc công việc.  
**Hoạt động**: Sinh viên lập Test Report giả định cho 5 test case của Todo App.  

---

#### Slide 9: Lưu Ý Test Report Trong Todo App
**Nội dung chính**:  
- **Chính xác**: Số test case và lỗi phải đúng.  
- **Hữu ích**: Khuyến nghị cụ thể (sửa lỗi, kiểm tra trình duyệt).  
- **Kịp thời**: Gửi trước hạn phát hành.  
**Ví dụ**:  
- Todo App: Báo cáo nêu lỗi giao diện, đề xuất kiểm tra trên mobile.  
**Hoạt động**: Thảo luận cách làm Test Report thuyết phục trong Todo App.  

---

#### Slide 10: Thách Thức Test Report Trong Todo App
**Nội dung chính**:  
- **Dữ liệu thiếu**: Kết quả kiểm thử trình duyệt chưa đầy đủ.  
- **Áp lực thời gian**: Báo cáo cần hoàn thành trong 1 ngày.  
- **Giải pháp**:  
  - Sử dụng mẫu báo cáo chuẩn.  
  - Tự động hóa thu thập dữ liệu từ TestRail.  
**Ví dụ**:  
- Todo App: Thách thức khi báo cáo lỗi hiệu suất do thiếu dữ liệu lớn.  
**Hoạt động**: Đề xuất cách cải thiện Test Report cho Todo App.  

---

## Phần 2: Tài Liệu Bài Tập Thực Hành

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
- **Định dạng**: File markdown hoặc Word, đặt tên theo mẫu: `[Họ_Tên]_Manual_T:template:esting_Assignment.md`.  
- **Thời hạn**: 1 tuần sau buổi học.  
- **Đánh giá**:  
  - Tính đầy đủ: Bao phủ yêu cầu bài tập.  
  - Tính chính xác: Nội dung đúng theo mẫu slide.  
  - Tính sáng tạo: Ví dụ thực tế, giải pháp đề xuất.  

---

## Phần 3: Đề Xuất Chuyển Slide Thành PowerPoint

Dưới đây là hướng dẫn và pseudocode để chuyển các slide từ markdown sang PowerPoint, đảm bảo giữ cấu trúc và nội dung.

### Hướng Dẫn Chuyển Đổi
1. **Chuẩn bị công cụ**:  
   - Sử dụng Microsoft PowerPoint hoặc Google Slides.  
   - Cài đặt công cụ chuyển đổi markdown sang PowerPoint (nếu muốn tự động hóa), ví dụ: `pandoc`.  
2. **Cấu trúc slide**:  
   - Mỗi slide markdown (tiêu đề, nội dung chính, ví dụ, hoạt động) tương ứng với 1 slide PowerPoint.  
   - **Tiêu đề slide**: Dùng tiêu đề markdown (ví dụ: "Test Plan Là Gì?").  
   - **Nội dung**: Dùng danh sách bullet từ "Nội dung chính".  
   - **Ví dụ/Hoạt động**: Đặt trong khung riêng hoặc ghi chú (notes) của slide.  
3. **Thiết kế**:  
   - Sử dụng template PowerPoint đơn giản (màu sắc trung tính, font Arial/Calibri).  
   - Thêm logo trường hoặc hình minh họa (ví dụ: giao diện Todo App).  
4. **Tự động hóa (nếu cần)**:  
   - Dùng `pandoc` để chuyển markdown sang `.pptx`.  
   - Cài đặt: `pip install pandoc`, sau đó chạy lệnh:  
     ```
     pandoc -t pptx Lecture_1_Introduction_to_Software_Testing.md -o Lecture_1.pptx
     ```
   - Kiểm tra và chỉnh sửa giao diện trong PowerPoint.  
5. **Lưu ý**:  
   - Kiểm tra định dạng bullet, tiêu đề trong PowerPoint.  
   - Thêm hình ảnh minh họa (ví dụ: ảnh chụp giao diện Todo App).  

### Pseudocode Chuyển Đổi
```
// Hàm chuyển markdown sang PowerPoint
Function ConvertMarkdownToPowerPoint(markdownFile, outputPptx):
    // Khởi tạo PowerPoint
    ppt = InitializePowerPoint()
    slideLayout = ppt.SlideLayouts[SimpleSlide] // Template slide đơn giản

    // Đọc file markdown
    markdownContent = ReadFile(markdownFile)
    slides = SplitMarkdownBySlide(markdownContent) // Tách theo tiêu đề slide

    // Lặp qua từng slide trong markdown
    For each slide in slides:
        newSlide = ppt.Slides.AddSlide(slideLayout)
        
        // Lấy tiêu đề slide
        title = ExtractSlideTitle(slide) // Ví dụ: "Test Plan Là Gì?"
        AddTextToSlideTitle(newSlide, title, Font="Arial", Size=24)

        // Lấy nội dung chính (bullet points)
        content = ExtractContent(slide, "Nội dung chính")
        AddBulletPoints(newSlide, content, Font="Arial", Size=18)

        // Lấy ví dụ
        example = ExtractContent(slide, "Ví dụ")
        AddTextBox(newSlide, example, Position="BottomLeft", Style="Italic")

        // Lấy hoạt động
        activity = ExtractContent(slide, "Hoạt động")
        AddNotes(newSlide, activity) // Thêm vào ghi chú slide

    // Lưu file PowerPoint
    SavePowerPoint(ppt, outputPptx)
    Return outputPptx
End Function

// Ví dụ sử dụng
ConvertMarkdownToPowerPoint("Lecture_1_Introduction_to_Software_Testing.md", "Lecture_1.pptx")
```

### Hướng Dẫn Thực Hiện Thủ Công
1. **Mở PowerPoint**: Tạo file mới, chọn template đơn giản.  
2. **Tạo slide**:  
   - Slide 1: Tiêu đề bài giảng (ví dụ: "Bài Giảng 1: Giới Thiệu Về Kiểm Thử Phần Mềm").  
   - Slide tiếp theo: Sao chép tiêu đề và nội dung từ markdown.  
   - Sử dụng bullet points cho "Nội dung chính".  
   - Thêm text box cho "Ví dụ" và ghi chú cho "Hoạt động".  
3. **Định dạng**:  
   - Tiêu đề: Font Arial, size 24, bold.  
   - Nội dung: Font Arial, size 18, bullet points.  
   - Ví dụ: Font Arial, size 16, italic, khung viền.  
4. **Hình ảnh**: Thêm ảnh minh họa (giao diện Todo App, biểu đồ kiểm thử).  
5. **Lưu file**: Đặt tên theo mẫu (ví dụ: `Lecture_1_Introduction.pptx`).  

---

## Hướng Dẫn Sử Dụng Trong Workspace
1. **Lưu và tải file**:
   - Lưu file trên thành `Supplementary_Lecture_Materials.md` và tải lên Workspace trong Grok.
2. **Viết Prompt để mở rộng**:
   - Nếu cần bổ sung, dùng prompt như:
     ```
     Tôi đã tải file "Supplementary_Lecture_Materials.md" vào Workspace. Vui lòng:
     1. Thêm 2 slide vào mỗi file về công cụ kiểm thử (TestRail, Jira) liên quan đến Todo App.
     2. Tạo bài tập nhóm (4-5 sinh viên) để thực hành kiểm thử thủ công trên Todo App.
     3. Cung cấp template PowerPoint (.pptx) mẫu cho các slide.
     Đầu ra: File markdown chứa slide bổ sung, bài tập nhóm, và link template.
     ```
3. **Kiểm tra và tinh chỉnh**:
   - Xem kết quả trong Grok Studio, chỉnh sửa slide hoặc bài tập nếu cần.

---

### Lưu Ý
- **Slide bổ sung**: 5 slide mỗi file, dùng Todo App để minh họa, đảm bảo liên quan đến nội dung gốc nhưng khác Notepad Cải Tiến.
- **Bài tập thực hành**: Thiết kế để sinh viên áp dụng lý thuyết, sử dụng Todo App làm bối cảnh, với hướng dẫn rõ ràng.
- **Chuyển PowerPoint**: Cung cấp cả cách thủ công và tự động (pandoc), với pseudocode chi tiết.
- Nếu bạn cần thêm slide, bài tập nhóm, template PowerPoint, hoặc nội dung cụ thể hơn, hãy cung cấp chi tiết để tôi hỗ trợ!

Bạn có muốn tôi tạo thêm nội dung, điều chỉnh bài tập, hoặc cung cấp template PowerPoint mẫu không?