# Simple Note App

Ứng dụng ghi chú đơn giản sử dụng Flutter và SQLite.
Lab 5 - Trần Đại Nghĩa

## Mô tả dự án

App cho phép tạo ghi chú với tiêu đề và nội dung, lưu trữ bằng SQLite ngay trên máy. Dùng Provider để cập nhật giao diện tự động khi có thay đổi.

### Tính năng chính

- Thêm ghi chú mới (tiêu đề + nội dung)
- Xem danh sách ghi chú dạng thẻ, bo tròn góc
- Sửa ghi chú (nhấn vào thẻ để sửa)
- Xóa ghi chú (có hộp thoại xác nhận tránh xóa nhầm)
- Lưu trữ cục bộ bền vững (SQLite)
- Tự động cập nhật thời gian tạo và sửa

## Ảnh chụp màn hình

(chụp ảnh từ điện thoại hoặc emulator rồi bỏ vào đây)

- Màn hình chính
  <img src="link_anh_1.png" />

- Màn hình tạo ghi chú
  <img src="link_anh_2.png" />

- Xác nhận xóa
  <img src="link_anh_3.png" />

## Cách chạy dự án

Yêu cầu:
- Flutter SDK >= 3.10.4
- Android Studio / VS Code
- Thiết bị Android (thật hoặc giả lập)

```bash
# clone repo
git clone https://github.com/adnosnghia/simple_note_app_trandainghia.git
cd simple_note_app_trandainghia

# cài dependencies
flutter pub get

# chạy app
flutter run
```

**Không cần API key hay file .env gì hết, chạy là được.**

## Cấu trúc dự án

```
lib/
├── main.dart
├── models/
│   └── note.dart
├── database/
│   └── db_helper.dart
├── providers/
│   └── note_provider.dart
├── screens/
│   ├── home_page.dart
│   └── note_editor_screen.dart
└── widgets/
    └── note_card.dart
```

## Công nghệ sử dụng

- Flutter - framework UI
- Provider - quản lý state (ChangeNotifier)
- sqflite - cơ sở dữ liệu SQLite
- path_provider - lấy đường dẫn lưu file database
- path - nối đường dẫn file
- intl - định dạng ngày tháng

## Hạn chế đã biết

- Chưa có tìm kiếm ghi chú
- Chưa có phân loại (category/tag)
- Chưa có dark mode
- Không có backup dữ liệu ra file

## License

Sinh viên: Trần Đại Nghĩa
