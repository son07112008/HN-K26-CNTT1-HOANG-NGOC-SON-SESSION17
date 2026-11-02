Phần 1: Phân tích lỗi sai của Nam
1.	Sai về DNS: Nếu DNS không tìm thấy IP, trình duyệt sẽ báo lỗi DNS_PROBE_FINISHED_NXDOMAIN chứ không thể kết nối đến server để nhận mã 500.
2.	Sai về mã 500: Lỗi 500 chứng tỏ máy tính đã phân giải xong DNS và kết nối thành công tới Server. Vấn đề nằm ở chỗ Server/Database bị sập, hoàn toàn không phải do mạng nhà Nam hỏng hay do lỗi DNS để mà đổi sang 8.8.8.8.
Phần 2: Luồng dữ liệu thực tế
•	DNS Lookup a-> TCP/TLS Handshake -> HTTP Request (Thành công đến server) -> Server Error (500) do backend/database gặp sự cố nội bộ.

