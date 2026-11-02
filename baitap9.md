Phần 1: Phân tích kiến trúc đa Profile

Nguyên nhân văng phiên đăng nhập (Session Conflict): Dùng chung 1 Profile đồng nghĩa với việc dùng chung thư mục User Data. Khi người khác đăng nhập tài khoản khác (PTIT, GitHub), các thẻ Token/Cookie định danh bị ghi đè hoặc xung đột, khiến hệ thống CarePulse tự động đăng xuất tài khoản của Bác sĩ trực để bảo mật.

Mô hình 3 Profile chuyên biệt:

CarePulse Clinic (Xanh dương): Dành cho Bác sĩ trực chính (lưu lịch sử, cookie, extension y tế riêng).

Medical Support (Xanh ngọc): Dành cho Điều dưỡng phụ tá (tác nghiệp hành chính).

Sandbox / Training (Cam/Xám): Dành cho sinh viên thực tập, học tập cá nhân.

Phần 2: Thiết kế Bookmark & An toàn bảo mật
Cây thư mục Bookmark chuẩn (Ctrl + Shift + O):

01_CarePulse_Clinic: Chứa các link quản lý ca trực, kê đơn, bệnh án nội trú, BHYT.

02_Pharma_Portal: Chứa link Tra cứu Dược thư, tương tác thuốc, danh mục BHYT.

03_Medical_Tools: Chứa công cụ tính BMI, quy đổi xét nghiệm, ICD-10, TeleHealth.

Mẹo Favicon-Only: Nhấp chuột phải vào Bookmark ➔ Chọn Chỉnh sửa ➔ Xóa sạch tên (để trống), chỉ giữ lại biểu tượng logo giúp thanh công cụ gọn gàng gấp 3 lần.

Xử lý Bẫy an ninh:

Khi khách mượn máy 30 phút, bắt buộc dùng Guest Profile (hoặc Incognito) để cô lập hoàn toàn dữ liệu.

Cảnh báo nguy cơ: Tuyệt đối không bật Cloud Sync tài khoản cá nhân lên máy tính phòng khám dùng chung để tránh làm lộ mật khẩu, dữ liệu y tế và thông tin bệnh nhân ra ngoài.