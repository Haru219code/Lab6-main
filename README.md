# SIMPLE MUZIK - OFFLINE MUSIC PLAYER

---

## GIỚI THIỆU DỰ ÁN
Simple Muzik là một ứng dụng phát nhạc offline chuyên nghiệp được phát triển trên nền tảng Flutter. Ứng dụng mang đến trải nghiệm nghe nhạc mượt mà, giao diện hiện đại mang phong cách Dark Mode và khả năng quản lý thư viện âm thanh toàn diện ngay trên thiết bị di động.

Demo: https://drive.google.com/drive/folders/1_nrGDmpEKAVGR9obwzgaiaHI4ddNwaqg?hl=vi
---

## TÍNH NĂNG NỔI BẬT

* **Quản lý thư viện nhạc:** Tự động quét các tệp âm thanh có sẵn trong thiết bị, hỗ trợ công cụ tìm kiếm nhanh và sắp xếp thông minh theo Tên bài, Nghệ sĩ hoặc Ngày thêm mới nhất.
<img width="389" height="850" alt="{AD4556A8-0F10-48AA-8B6F-E53F2F19D248}" src="https://github.com/user-attachments/assets/3e95441d-6edd-4247-b294-c6a5f0e6709b" />



* **Quản lý Playlist cá nhân:** Người dùng có thể tự do tạo mới, đổi tên, xóa danh sách phát, cũng như thêm/bớt các bài hát yêu thích vào Playlist dễ dàng.
<img width="395" height="859" alt="{5F39779A-C8EE-4AB9-85D9-9A56967573B4}" src="https://github.com/user-attachments/assets/9b9a4a05-2a34-4541-ae9b-5c0fd9eb9213" />



* **Điều khiển âm thanh toàn diện:** Đầy đủ các thao tác cơ bản (Phát, Tạm dừng, Chuyển bài, Tua). Tích hợp thanh trượt điều chỉnh âm lượng (Volume) và thay đổi tốc độ phát nhạc (từ 0.5x đến 2.0x).

<img width="398" height="858" alt="{38A63FEA-8BF8-4939-9BFF-1BBABE6A8CAE}" src="https://github.com/user-attachments/assets/39920f32-86f5-44f5-b2a2-587c04667423" />


* **Các chế độ phát nhạc:** Hỗ trợ Trộn bài (Shuffle) ngẫu nhiên và Lặp lại (Repeat All, Repeat One, Repeat Off).

<img width="385" height="313" alt="{79A1A9F4-9FD5-4E2E-9C90-D3C27D11B82D}" src="https://github.com/user-attachments/assets/3ba2a35b-6875-41ea-8754-905902548df3" />


* **Phát nhạc chạy nền (Background Playback):** Âm nhạc không bao giờ dừng lại. Ứng dụng tiếp tục phát nhạc ngay cả khi bị ẩn xuống nền hoặc khi khóa màn hình, kèm theo trình điều khiển trực tiếp trên thanh thông báo hệ thống.

<img width="338" height="174" alt="{F9BE3EEE-3331-46EB-9F84-1CB711E33314}" src="https://github.com/user-attachments/assets/9c305e22-3194-4ee4-9b82-e3ba84f1cfb0" />


* **Lưu trữ trạng thái thông minh:** Ứng dụng tự động ghi nhớ bài hát đang nghe dở, vị trí thời gian bài hát, cấu hình âm lượng và danh sách Playlist. Khi khởi động lại, mọi thứ vẫn ở nguyên vị trí cũ.

---

## CÔNG NGHỆ VÀ THƯ VIỆN SỬ DỤNG

- **Ngôn ngữ & Khung làm việc:** Dart, Flutter
- **Quản lý trạng thái:** Provider
- **Lõi xử lý âm thanh:** just_audio, just_audio_background, audio_service
- **Truy xuất dữ liệu thiết bị:** on_audio_query, permission_handler
- **Lưu trữ dữ liệu cục bộ:** shared_preferences
- **Tiện ích lập trình phản ứng:** rxdart

---

## CẤU TRÚC THƯ MỤC

- **models/**: Định nghĩa cấu trúc dữ liệu cho bài hát và danh sách phát.
- **providers/**: Bộ não xử lý logic và quản lý trạng thái của Audio và Playlist.
- **screens/**: Giao diện các màn hình chính (Home, Now Playing, Playlists...).
- **services/**: Các dịch vụ cốt lõi (xử lý trình phát nhạc, xin quyền, quét nhạc).
- **widgets/**: Các thành phần giao diện tái sử dụng (Song Tile, Mini Player...).
- **main.dart**: Điểm khởi chạy ứng dụng, cấu hình dịch vụ nền.

---

## HƯỚNG DẪN CÀI ĐẶT VÀ SỬ DỤNG

1. Clone hoặc tải mã nguồn về máy tính.
2. Mở terminal tại thư mục dự án và chạy lệnh: flutter pub get để tải các thư viện.
3. Kết nối thiết bị Android thật hoặc máy ảo. Đảm bảo thiết bị đã có sẵn một số tệp nhạc mp3.
4. Khởi chạy ứng dụng bằng lệnh: flutter run
5. Ở lần mở đầu tiên, hãy cấp quyền truy cập bộ nhớ khi ứng dụng yêu cầu để hệ thống có thể quét nhạc.
