# 📚 NXT Retro BookNest

**Đọc truyện tranh và sách ngay trên máy chơi game cầm tay.**

[English](README.md) · [Hướng dẫn sử dụng](docs/HUONG_DAN_SU_DUNG.md) · [Hướng dẫn cài đặt](docs/CAI_DAT.md)

BookNest là một tủ sách bỏ túi cho máy chơi game cầm tay: đọc truyện tranh, truyện chữ và sách, online hoặc từ thẻ nhớ. Có thể xoay màn hình, chọn kiểu đọc, chỉnh chữ theo ý thích và quay lại đúng chỗ đang đọc.

**Phiên bản:** 1.0.2 · **Dự án:** NXT Retro / [SpringThong](https://github.com/SpringThong)

## Tải ứng dụng

Các gói cài sẽ được tác giả đính kèm trong **[Releases](https://github.com/SpringThong/NXT-Retro-BookNest/releases)**. Nếu chưa thấy ZIP đúng ROM thì bản cài đó chưa được đăng tại đây.

| Máy | ROM | Gói cài 1.0.2 |
| --- | --- | --- |
| TrimUI Brick Pro | Stock | `NXT_Retro_BookNest_v1.0.2_BrickPro_Stock.zip` |
| TrimUI Brick Pro | NX Redux | `NXT_Retro_BookNest_v1.0.2_BrickPro_NXRedux.zip` |
| TrimUI Brick Pro | NextUI | `NXT_Retro_BookNest_v1.0.2_BrickPro_NextUI.zip` |
| TrimUI Brick Pro | Knulli | `NXT_Retro_BookNest_v1.0.2_BrickPro_Knulli.zip` |
| TrimUI Brick Pro | muOS | `NXT_Retro_BookNest_v1.0.2_BrickPro_MuOS.zip` |
| R36S | DarkOS / dArkOS | `NXT_Retro_BookNest_v1.0.2_R36S_DarkOS.zip` |

Chỉ cần chọn **một gói đúng máy và ROM**. Mục “Source code” GitHub tự tạo chỉ tải tài liệu của repo này, không phải gói cài ứng dụng.

## Có gì trong BookNest?

- **Đọc offline:** duyệt theo thư mục; mở ảnh, CBZ/ZIP, TXT, EPUB, MOBI/PRC được hỗ trợ và PDF.
- **Đọc online:** thêm URL hoặc chọn nguồn gợi ý trong app; duyệt thể loại, tìm truyện, chọn chương và chuyển chương kế khi nguồn cung cấp liên kết.
- **Đọc như sách:** bìa, mục lục, một trang, hai trang hoặc cuộn; hiệu ứng lật trang cho nội dung chữ được hỗ trợ.
- **Chỉnh cách đọc:** font, cỡ chữ, giãn dòng, lề, tương phản, màu chữ và nền; có nền sáng, tối, giấy ngà và trắng đen.
- **Xoay và cuộn:** xoay bốn hướng, zoom, tự cuộn và đổi tốc độ ngay khi đọc; tuỳ chọn bật/tắt và phạm vi zoom của analog phải.
- **Đọc tiếp dễ hơn:** lưu vị trí, đánh dấu, tìm chương và mở mục lục từ truyện đang đọc trong Tủ sách.
- **Tiếng Việt / English:** chọn ngôn ngữ giao diện trong Cài đặt; kèm font bù nhiều hệ chữ.
- **Tối ưu 1.0.2:** dàn trang chữ từng phần, dùng lại ảnh trang khi cuộn/zoom, ưu tiên thao tác đang đọc; nạp trước 5–10 trang, mặc định 8.

Các gói giữ cùng tính năng và giao diện đọc. Launcher, icon, hiển thị và điều khiển được điều chỉnh theo ROM; trên R36S, giao diện được đưa xuống màn hình 640×480.

## Bắt đầu nhanh

1. Tải đúng ZIP và cài theo [bảng đường dẫn của từng ROM](docs/CAI_DAT.md).
2. Mở app từ Apps, Tools, Applications hoặc Ports.
3. Đọc offline: vào **Tải về / Offline**, mở thư mục chứa sách rồi bấm A.
4. Đọc online: vào **Web truyện**, thêm nguồn trước, sau đó chọn truyện và chương.
5. Khi đang đọc, bấm **START** để mở mục lục, font, giao diện đọc và tốc độ tự cuộn.

Xem [hướng dẫn sử dụng đầy đủ](docs/HUONG_DAN_SU_DUNG.md) để biết các phím tắt, tuỳ chọn zoom, PDF và cách tiếp tục đọc.

## Khi nâng cấp

Thoát app, chép đầy đủ gói mới và **giữ nguyên thư mục `data`**. Không chỉ chép riêng tệp thực thi. Với Knulli/DarkOS, làm mới danh sách Ports sau lần mở đầu để nạp icon; với NextUI, bật Game Art để hiện ảnh ứng dụng.

## Một vài điều cần biết

MOBI 6/7 và PalmDOC/PRC không DRM được hỗ trợ; KF8-only/AZW3 và sách có DRM chưa hỗ trợ. PDF có thể đọc trang gốc hoặc dàn lại chữ khi có lớp văn bản phù hợp; app chưa có OCR.

Nguồn online có thể đổi tên miền, đổi cấu trúc hoặc giới hạn truy cập. Các chức năng tìm kiếm và chuyển chương phụ thuộc dữ liệu nguồn cung cấp. Có thể đổi URL nguồn đã lưu trong app khi website đổi tên miền.

App đặt mục tiêu 60 Hz khi thao tác, có lựa chọn 30 Hz trong Cài đặt. NX Redux đã có phản hồi sử dụng tốt; các gói ROM khác đã build và kiểm tra tự động nhưng vẫn cần thử trên máy thật. Chưa có phép đo FPS, GPU và nhiệt độ cho cả sáu cấu hình.

## Góp ý và báo lỗi

Mở [Issues](https://github.com/SpringThong/NXT-Retro-BookNest/issues), ghi rõ máy, ROM/phiên bản, phiên bản app và các bước gặp lỗi. Có thể gửi `data/launch.log` và `data/BookNest.log` trong thư mục app; hãy bỏ URL riêng tư và thông tin cá nhân trước khi đăng công khai.

[Thay đổi bản 1.0.2](CHANGELOG.md) · [Cài đặt](docs/CAI_DAT.md) · [Hướng dẫn sử dụng](docs/HUONG_DAN_SU_DUNG.md)
