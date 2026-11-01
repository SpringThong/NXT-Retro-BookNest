# Cài NXT Retro BookNest 1.0.2

[Trang giới thiệu](../README.vi.md) · [Hướng dẫn sử dụng](HUONG_DAN_SU_DUNG.md) · [English](INSTALLATION.md)

## Chọn gói đúng ROM

Tải tại [Releases](https://github.com/SpringThong/NXT-Retro-BookNest/releases). Mỗi máy chỉ cần gói phù hợp với ROM đang dùng.

| Máy / ROM | Giải nén vào | Tệp cần có sau khi cài | Mở từ |
| --- | --- | --- | --- |
| Brick Pro / Stock | Gốc thẻ nhớ | `Apps/NXT_Retro_BookNest/launch.sh` | Apps |
| Brick Pro / NX Redux | Gốc thẻ nhớ | `Tools/NXT_Retro_BookNest.pak/launch.sh` | Tools |
| Brick Pro / NextUI | Gốc thẻ nhớ | `Tools/tg5040/NXT_Retro_BookNest.pak/launch.sh` | Tools |
| Brick Pro / Knulli | Gốc SHARE, tương ứng `/userdata` | `roms/ports/NXT_Retro_BookNest.sh` | Ports |
| Brick Pro / muOS | Gốc thẻ chứa MUOS | `MUOS/application/NXT_Retro_BookNest/mux_launch.sh` | Applications |
| R36S / DarkOS | Gốc EASYROMS trên thẻ đang chứa ROM | `ports/NXT_Retro_BookNest.sh` | Ports |

Giữ nguyên cấu trúc thư mục trong ZIP. Stock dùng tên thư mục có dấu gạch dưới; không đổi thành tên có khoảng trắng. Không cài gói của ROM khác để thử thay thế.

## Cài lần đầu

1. Thoát ứng dụng trên máy trước khi tháo thẻ hoặc thay tệp.
2. Giải nén ZIP đúng vị trí trong bảng.
3. Chép đủ thư mục ứng dụng, gồm fonts, bộ đọc PDF và các tệp đi kèm.
4. Gắn thẻ lại, mở app từ mục tương ứng. Với Ports, làm mới danh sách nếu chưa thấy tên app.

Không cần cài Python hoặc PortMaster để chạy BookNest. Các gói Knulli/muOS/DarkOS dùng SDL2 ARM64 của ROM. Gói có sẵn bộ đọc PDF riêng.

## Cập nhật và chuyển dữ liệu

Thoát app rồi chép đè các tệp ứng dụng mới. **Giữ `data` trong thư mục app** để giữ nguồn, lịch sử, đánh dấu, cài đặt và sách tải về. Gói cài không chứa dữ liệu cá nhân.

Nếu chuyển ROM, hãy sao lưu `data` trước. Kiểm tra lại đường dẫn sách sau khi chuyển vì vị trí gắn thẻ có thể khác. Không xoá dữ liệu cũ trước khi xác nhận app mới đọc được.

## Sách offline ở đâu?

- Các bản trên Stock/NX Redux/NextUI có lối tắt tới thư mục `Books` ở gốc thẻ.
- Knulli/DarkOS lấy đường dẫn từ vị trí cài; DarkOS dùng được cả thẻ ROM đang gắn tại `/roms` hoặc `/roms2`.
- muOS lấy đường dẫn lưu trữ từ thiết lập của ROM khi có hàm hệ thống phù hợp.
- Sách tải bên trong app ở `data/books`.

Vào **Tải về / Offline** và bấm **Y** để mở Books mà launcher chọn. Bạn vẫn có thể duyệt sang thư mục khác.

## Icon

| ROM | Cách hiện icon |
| --- | --- |
| Stock | Gói có `config.json`, `icon.png` và `icontop.png`. |
| NX Redux | Có icon và mục **Khôi phục logo NX Redux**; cơ chế sửa chỉ áp dụng với launcher được nhận diện. |
| NextUI | Có ảnh `.media` bên cạnh `.pak`; bật Game Art trong NextUI để hiện ảnh khi chọn app. |
| muOS | Có glyph và khai báo icon cho Applications. |
| Knulli / DarkOS | App đăng ký riêng mục BookNest trong danh sách Ports; thoát và làm mới danh sách sau lần mở đầu. |

Các ROM ngoài NX Redux có mục **Khôi phục icon ứng dụng** trong Cài đặt. Việc sửa icon giữ các mục khác trong gamelist; nếu metadata lỗi hoặc không ghi được, app ghi lý do vào log và vẫn cho mở trình đọc.

## Không mở được app

Kiểm tra đúng máy, đúng ROM và đúng đường dẫn trong bảng. Thử chép lại đầy đủ gói; đừng chỉ chép tệp `nxt-booknest`. Với Stock, kiểm tra tên thư mục không có khoảng trắng.

Log nằm ở `data/launch.log` và `data/BookNest.log` trong thư mục app. Gửi kèm tên ROM/phiên bản và mô tả khi nào app thoát. Giữ lại `data` để tránh mất lịch sử trong quá trình kiểm tra.
