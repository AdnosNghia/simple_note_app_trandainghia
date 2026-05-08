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


- Màn hình chính

<img width="488" height="1021" alt="{D3F745D2-D6B0-4D5D-AB5D-49AF8E569BBF}" src="https://github.com/user-attachments/assets/7a9f046e-b8d0-4541-a4d4-a9eec323eec9" />


- Màn hình tạo ghi chú

<img width="498" height="1025" alt="{5DDF1EFF-991C-4FB2-A655-4E400F4788BE}" src="https://github.com/user-attachments/assets/07307ffb-1b88-446f-a228-72e51ca4cb28" />


- Xác nhận xóa
<img width="511" height="1015" alt="{21C569F6-9F23-449C-B215-FB75AA6D48E6}" src="https://github.com/user-attachments/assets/6eba78eb-6e43-4f1d-a00b-026dbd66a98b" />


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
