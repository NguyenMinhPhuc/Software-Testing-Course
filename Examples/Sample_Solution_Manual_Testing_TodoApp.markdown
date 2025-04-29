# Bài Giải Mẫu: Thực Hành Kiểm Thử Thủ Công Trên Todo App

## Giới Thiệu
Tài liệu này cung cấp bài giải mẫu cho bài tập nhóm trong `Group_Assignment_Manual_Testing_TodoApp.md`. Mục tiêu là minh họa cách thực hiện các nhiệm vụ kiểm thử thủ công cho **Todo App** (ứng dụng web quản lý công việc), bao gồm lập Test Plan, viết Test Case, thực thi kiểm thử, và lập Test Report. Sinh viên có thể tham khảo để hiểu cách áp dụng lý thuyết từ các bài giảng.

- **Ứng dụng**: Todo App cho phép tạo, chỉnh sửa, xóa công việc, gắn thẻ ưu tiên (Cao, Trung, Thấp), và lọc công việc theo trạng thái (Hoàn thành, Chưa hoàn thành) hoặc ưu tiên.
- **PRD giả định**: Yêu cầu chức năng (tạo, xóa, lọc công việc), phi chức năng (hiệu suất lọc < 1 giây, tương thích Chrome/Firefox).
- **Môi trường**: Chrome, Firefox trên Windows 10.

## Nhiệm Vụ 1: Lập Test Plan

### Test Plan Cho Todo App
**1. Mục tiêu kiểm thử**:  
- Đảm bảo các tính năng tạo, xóa, lọc công việc hoạt động đúng theo PRD.  
- Xác minh tương thích giao diện trên Chrome và Firefox.  
- Đạt tỷ lệ pass 90% cho Test Case và không có lỗi nghiêm trọng.

**2. Phạm vi kiểm thử**:  
- **Trong phạm vi**:  
  - Tính năng: Tạo, chỉnh sửa, xóa công việc; lọc theo trạng thái và ưu tiên.  
  - Yêu cầu phi chức năng: Hiệu suất lọc (< 1 giây), tương thích Chrome/Firefox.  
- **Ngoài phạm vi**:  
  - Tích hợp với Google Calendar.  
  - Kiểm thử trên các trình duyệt khác (Safari, Edge).  

**3. Phương pháp kiểm thử**:  
- Kiểm thử thủ công hộp đen, theo mô hình Agile (kiểm thử từng sprint).  
- Sử dụng Test Case để xác minh yêu cầu chức năng và phi chức năng.

**4. Tài nguyên**:  
- **Công cụ**: Excel (quản lý Test Case), Jira (theo dõi lỗi).  
- **Môi trường**: Windows 10, Chrome (phiên bản mới nhất), Firefox (phiên bản mới nhất).  
- **Nhân sự**: 4-5 QA (vai trò: lập Test Plan, viết Test Case, thực thi, báo cáo).

**5. Tiêu chí hoàn thành**:  
- 90% Test Case passed.  
- 95% yêu cầu được bao phủ (theo ma trận truy xuất).  
- Tất cả lỗi nghiêm trọng (Critical, High) được sửa.  
- Lỗi thấp (Low) được ghi nhận và lên kế hoạch sửa trong phiên bản sau.

**6. Rủi ro và giảm thiểu**:  
- **Rủi ro**: Lỗi tương thích trên Firefox do khác biệt rendering.  
  - **Giảm thiểu**: Kiểm thử song song trên Chrome và Firefox từ sớm.  
- **Rủi ro**: Hiệu suất lọc chậm khi có >1,000 công việc.  
  - **Giảm thiểu**: Mô phỏng dữ liệu lớn (1,000 công việc) trong môi trường kiểm thử.

**7. Lịch trình**:  
- Phân tích PRD: 1 ngày.  
- Viết Test Case: 2 ngày.  
- Thực thi kiểm thử: 2 ngày.  
- Lập Test Report: 1 ngày.

---

## Nhiệm Vụ 2: Viết Test Case

Dưới đây là 10 Test Case mẫu cho các tính năng **tạo công việc**, **xóa công việc**, và **lọc công việc**, dựa trên yêu cầu kiểm thử (TR):

### Yêu cầu kiểm thử (TR)
- TR-001: Tạo công việc với tiêu đề tối đa 200 ký tự.  
- TR-002: Xóa công việc, yêu cầu xác nhận trước khi xóa.  
- TR-003: Lọc công việc theo trạng thái "Hoàn thành" hoặc "Chưa hoàn thành".  
- TR-004: Tương thích giao diện trên Chrome và Firefox.

### Test Case
| ID      | Mô tả                                              | Điều kiện tiên quyết                       | Bước thực hiện                                                                 | Kết quả mong đợi                              |
|---------|----------------------------------------------------|--------------------------------------------|-------------------------------------------------------------------------------|-----------------------------------------------|
| TC-001  | Kiểm tra tạo công việc với tiêu đề hợp lệ          | Todo App chạy trên Chrome                  | 1. Mở Todo App. 2. Nhập tiêu đề "Họp nhóm". 3. Nhấn "Thêm".                   | Công việc "Họp nhóm" hiển thị trong danh sách. |
| TC-002  | Kiểm tra tạo công việc với tiêu đề rỗng            | Todo App chạy trên Chrome                  | 1. Mở Todo App. 2. Để trống tiêu đề. 3. Nhấn "Thêm".                          | Hiển thị thông báo lỗi "Tiêu đề không được để trống". |
| TC-003  | Kiểm tra tạo công việc với tiêu đề 200 ký tự       | Todo App chạy trên Chrome                  | 1. Mở Todo App. 2. Nhập tiêu đề 200 ký tự. 3. Nhấn "Thêm".                   | Công việc hiển thị đúng trong danh sách.       |
| TC-004  | Kiểm tra xóa công việc với xác nhận                | Todo App chạy trên Chrome, có 1 công việc  | 1. Chọn công việc. 2. Nhấn "Xóa". 3. Xác nhận "Có" trong hộp thoại.           | Công việc bị xóa khỏi danh sách.              |
| TC-005  | Kiểm tra xóa công việc nhưng hủy xác nhận          | Todo App chạy trên Chrome, có 1 công việc  | 1. Chọn công việc. 2. Nhấn "Xóa". 3. Chọn "Hủy" trong hộp thoại.              | Công việc vẫn hiển thị trong danh sách.       |
| TC-006  | Kiểm tra lọc công việc trạng thái "Hoàn thành"     | Todo App chạy trên Chrome, có 3 công việc (2 hoàn thành, 1 chưa) | 1. Chọn bộ lọc "Hoàn thành". 2. Xem danh sách.                        | Chỉ hiển thị 2 công việc hoàn thành.          |
| TC-007  | Kiểm tra lọc công việc trạng thái "Chưa hoàn thành" | Todo App chạy trên Chrome, có 3 công việc (2 hoàn thành, 1 chưa) | 1. Chọn bộ lọc "Chưa hoàn thành". 2. Xem danh sách.                   | Chỉ hiển thị 1 công việc chưa hoàn thành.     |
| TC-008  | Kiểm tra lọc công việc khi không có kết quả        | Todo App chạy trên Chrome, không có công việc hoàn thành | 1. Chọn bộ lọc "Hoàn thành". 2. Xem danh sách.                        | Hiển thị thông báo "Không có công việc phù hợp". |
| TC-009  | Kiểm tra tương thích giao diện trên Chrome         | Todo App chạy trên Chrome                  | 1. Mở Todo App. 2. Kiểm tra bố cục (nút, danh sách).                         | Giao diện hiển thị đúng, không lệch.          |
| TC-010  | Kiểm tra tương thích giao diện trên Firefox        | Todo App chạy trên Firefox                 | 1. Mở Todo App. 2. Kiểm tra bố cục (nút, danh sách).                         | Giao diện hiển thị đúng, không lệch.          |

---

## Nhiệm Vụ 3: Thực Thi Kiểm Thử

Giả định nhóm đã thực thi 10 Test Case trên Todo App (môi trường mô phỏng). Dưới đây là kết quả và lỗi phát hiện:

### Kết quả kiểm thử
| ID      | Kết quả thực tế                              | Pass/Fail |
|---------|----------------------------------------------|-----------|
| TC-001  | Công việc hiển thị đúng                      | Pass      |
| TC-002  | Hiển thị thông báo lỗi                       | Pass      |
| TC-003  | Công việc hiển thị đúng                      | Pass      |
| TC-004  | Công việc bị xóa                             | Pass      |
| TC-005  | Công việc vẫn hiển thị                       | Pass      |
| TC-006  | Chỉ hiển thị 2 công việc hoàn thành          | Pass      |
| TC-007  | Chỉ hiển thị 1 công việc chưa hoàn thành     | Pass      |
| TC-008  | Hiển thị thông báo đúng                      | Pass      |
| TC-009  | Giao diện hiển thị đúng                      | Pass      |
| TC-010  | Giao diện lệch, nút "Thêm" bị cắt trên Firefox | Fail      |

### Lỗi phát hiện
| ID      | Mô tả                                              | Mức độ   | Trạng thái |
|---------|----------------------------------------------------|----------|------------|
| BUG-001 | Giao diện lệch, nút "Thêm" bị cắt trên Firefox     | Thấp     | Chưa sửa   |
| BUG-002 | Lọc công việc chậm (>1 giây) với 1,000 công việc   | Cao      | Chưa sửa   |

**Ghi chú**: BUG-002 được phát hiện khi mô phỏng dữ liệu lớn (1,000 công việc), mặc dù không có Test Case cụ thể cho trường hợp này (nhóm tự kiểm tra bổ sung).

---

## Nhiệm Vụ 4: Lập Test Report

### Test Report Cho Todo App
**1. Thông tin chung**:  
- **Dự án**: Todo App.  
- **Phiên bản**: 1.0.  
- **Ngày kiểm thử**: 01/06/2025.  
- **Nhóm thực hiện**: Nhóm 1 (5 thành viên: Nguyễn Văn A, Trần Thị B, ...).

**2. Tóm tắt kết quả**:  
- **Số Test Case**: 10.  
- **Kết quả**: 9 Pass, 1 Fail (90% tỷ lệ Pass).  
- **Bao phủ yêu cầu**: 95% (4/4 TR được kiểm thử qua ma trận truy xuất).  
- **Lỗi phát hiện**: 2 lỗi (1 Cao, 1 Thấp).

**3. Phân tích lỗi**:  
| ID      | Mô tả                                              | Mức độ | Trạng thái | Test Case liên quan |
|---------|----------------------------------------------------|--------|------------|---------------------|
| BUG-001 | Giao diện lệch, nút "Thêm" bị cắt trên Firefox     | Thấp   | Chưa sửa   | TC-010             |
| BUG-002 | Lọc công việc chậm (>1 giây) với 1,000 công việc   | Cao    | Chưa sửa   | Không trực tiếp    |

**4. Ma trận truy xuất**:  
| TR-ID | Mô tả                                     | Test Case liên quan |
|-------|-------------------------------------------|---------------------|
| TR-001 | Tạo công việc với tiêu đề tối đa 200 ký tự | TC-001, TC-002, TC-003 |
| TR-002 | Xóa công việc, yêu cầu xác nhận           | TC-004, TC-005      |
| TR-003 | Lọc công việc theo trạng thái             | TC-006, TC-007, TC-008 |
| TR-004 | Tương thích giao diện Chrome/Firefox      | TC-009, TC-010      |

**5. Đánh giá và khuyến nghị**:  
- **Đánh giá**:  
  - Todo App đạt chất lượng tốt với 90% Test Case passed và 95% bao phủ yêu cầu.  
  - Tuy nhiên, lỗi hiệu suất (BUG-002) là nghiêm trọng, ảnh hưởng trải nghiệm người dùng với dữ liệu lớn.  
  - Lỗi giao diện (BUG-001) ít nghiêm trọng nhưng cần sửa để đảm bảo tính nhất quán.  
- **Khuyến nghị**:  
  - Sửa BUG-002 (tối ưu API lọc công việc) và kiểm thử lại với 1,000 công việc.  
  - Sửa BUG-001 (điều chỉnh CSS cho Firefox) trước phát hành.  
  - Thêm Test Case cho trường hợp dữ liệu lớn (ví dụ: lọc 1,000 công việc) trong lần kiểm thử tiếp theo.  
- **Quyết định**: Không nên phát hành cho đến khi BUG-002 được sửa.

**6. Phê duyệt**:  
- **Người lập báo cáo**: Nguyễn Văn A.  
- **Quản lý kiểm thử**: (Chờ phê duyệt).

---

## Lưu Ý Cho Sinh Viên
- **Cách sử dụng bài giải mẫu**:  
  - Tham khảo cấu trúc và nội dung của Test Plan, Test Case, và Test Report.  
  - Không sao chép nguyên văn; hãy tự viết dựa trên hiểu biết và sáng tạo của nhóm.  
- **Điểm khác biệt**:  
  - Bài giải mẫu giả định một số lỗi (BUG-001, BUG-002) để minh họa. Nhóm bạn có thể mô phỏng các lỗi khác hoặc thêm Test Case mới.  
  - Test Plan và Test Report có thể điều chỉnh phạm vi, tiêu chí, hoặc khuyến nghị dựa trên phân tích của nhóm.  
- **Tài liệu tham khảo**:  
  - Lecture_2_Building_Test_Plan.md (Slide 2, 3, 5-7).  
  - Lecture_4_Test_Case_Design.md (Slide 2, 3, 6-8).  
  - Lecture_5_Test_Report.md (Slide 2, 3, 6-8).