# ZMK Dongle Corne/Sofle

Đây là repo firmware tổng hợp, có hỗ trợ dongle rời cho máy tính không có Bluetooth.

## Sofle macOS keymap V1

Keymap nằm tại `config/sofle.keymap` và giữ nguyên thứ tự phần cứng 58 phím cùng hai nút nhấn encoder.

### Thumb cluster

```text
Trái:  Option | Command | NAV | Space | Backspace
Phải:  Delete | Enter   | SYM | Command | Option
```

### Layers

- `BASE`: QWERTY dành cho macOS.
- `NAV`: phím mũi tên, Home/End, Page Up/Page Down và các phím tắt Undo/Cut/Copy/Paste.
- `SYM`: số, ngoặc và ký hiệu thường dùng khi lập trình.
- `SYS`: giữ đồng thời `NAV + SYM` để chọn/xóa Bluetooth profile, chỉnh media/độ sáng hoặc reset.

### Encoders

- Encoder trái: tăng/giảm âm lượng.
- Encoder phải: Page Up/Page Down.

## Lưu ý trước khi flash

Nhánh `original-shop-keymap` giữ cấu hình gốc của shop. Sau khi GitHub Actions build thành công, tải đúng firmware Sofle và flash từng bên; không dùng artifact Corne hoặc Aurora Sofle.
