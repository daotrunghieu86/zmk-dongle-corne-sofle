# ZMK Dongle Corne/Sofle

Đây là repo firmware tổng hợp, có hỗ trợ dongle rời cho máy tính không có Bluetooth.

## Sofle macOS developer keymap V2

Keymap nằm tại `config/sofle.keymap` và giữ nguyên thứ tự phần cứng 58 phím cùng hai nút nhấn encoder.

### Thumb cluster

```text
Trái:  Option | Command | NAV | Enter | Backspace
Phải:  Delete | Space   | SYM | Command | Option
```

### Layers

- `BASE`: QWERTY dành cho macOS.
- `NAV`: browser history, mũi tên, word/line navigation, Page Up/Page Down và tab navigation.
- `SYM`: số, ngoặc và ký hiệu thường dùng khi lập trình.
- `SYS`: giữ đồng thời `NAV + SYM` để dùng F1–F12, Bluetooth, media, độ sáng, reset hoặc bật `MOUSE`.
- `MOUSE`: tại `SYS`, nhấn phím vật lý `M` để bật/tắt; có cursor, scroll, Back/Forward và ba nút chuột. Nhấn `Esc` hoặc `M` để thoát.

### Encoders

- Encoder trái: chuyển macOS Space/Workspace trước hoặc sau; nhấn để mở Mission Control.
- Encoder phải: chuyển tab trước hoặc sau; nhấn để đóng tab hiện tại.

### Đổi ngôn ngữ macOS

Giữ `NAV`, giữ phím vật lý `S` (Control), sau đó nhấn `Space`. Tổ hợp gửi `Control + Space` mà không cần một phím Globe riêng.

## Lưu ý trước khi flash

Nhánh `original-shop-keymap` giữ cấu hình gốc của shop. Sau khi GitHub Actions build thành công, tải đúng firmware Sofle và flash từng bên; không dùng artifact Corne hoặc Aurora Sofle.
