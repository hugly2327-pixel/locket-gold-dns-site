LOCKET GOLD — TRANG TẢI HỒ SƠ DNS (BẢN THỬ NGHIỆM TRIỂN KHAI)

Tệp:
- index.html: giao diện đen/vàng cho Safari trên iPhone.
- LocketGoldDNS.mobileconfig: hồ sơ DNS-over-TLS được dựng theo cấu hình đã cung cấp trong cuộc trò chuyện.
- README.txt: hướng dẫn.

LƯU Ý QUAN TRỌNG
1. Hồ sơ đặt DNS-over-TLS tới:
   ServerName: bb475f.dns.nextdns.io
   ServerAddresses: 45.90.28.0, 45.90.30.0
2. Không thể xác nhận chỉ từ file rằng NextDNS profile này còn hoạt động, thuộc tài khoản của bạn, hoặc có các bộ lọc nào đang bật. Hãy xác nhận trong bảng điều khiển NextDNS trước khi cài.
3. Đây là cấu hình DNS, không phải công cụ mở khóa Locket Gold.
4. Trang web không thể bỏ qua bước xác nhận của iOS.

KIỂM THỬ CỤC BỘ
- Giải nén ZIP.
- Mở index.html trên máy tính để kiểm tra giao diện/đường dẫn.
- Để kiểm thử iOS thực tế, hãy host cả index.html và LocketGoldDNS.mobileconfig trên cùng thư mục HTTPS rồi mở index.html trong Safari trên iPhone.

TRIỂN KHAI
- Đưa cả hai file lên cùng thư mục của dịch vụ hosting tĩnh có HTTPS (ví dụ GitHub Pages hoặc Cloudflare Pages).
- Không đổi tên file mobileconfig nếu chưa sửa href trong index.html.
- Nếu có thể cấu hình MIME type, dùng application/x-apple-aspen-config cho .mobileconfig.
- Sau khi mở trang trên iPhone, nhấn Tải cấu hình DNS; vào Cài đặt và tự xác nhận cài đặt. Nếu không cài trong thời hạn hiển thị của iOS, hồ sơ tải về có thể bị xóa tự động.

AN TOÀN
- Chỉ cài profile DNS mà bạn tin tưởng.
- Nếu muốn hoàn tác: Cài đặt > Cài đặt chung > VPN & Quản lý thiết bị > chọn profile > Xóa hồ sơ (tên mục có thể khác tùy phiên bản iOS).
