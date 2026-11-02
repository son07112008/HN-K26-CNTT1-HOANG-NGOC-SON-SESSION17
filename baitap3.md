Phần 1: Báo cáo phân tích Box Model
Nguyên nhân lỗi chồng lấn: Hai khung "Nội dung bài học" và "Danh sách video" bị đè lên nhau do khung video đang mang thuộc tính margin-right: -28px; (margin âm) làm kéo lệch vị trí hiển thị.

4 lớp Box Model: Gồm Content (vùng nội dung), Padding (15px), Border (2px solid red), và Margin (chứa giá trị âm gây lỗi).

Phần 2: Giải pháp khắc phục
Tại bảng Styles:

Sửa lại margin-right: -28px; thành margin-right: 15px; (hoặc 0) cho khung video.

Đảm bảo các khung đều có thêm thuộc tính box-sizing: border-box; để trình duyệt tự động tính toán chính xác kích thước, tránh làm vỡ giao diện chung của toàn trang PTIT-LMS.