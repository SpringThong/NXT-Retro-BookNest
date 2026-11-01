# 📚 NXT Retro BookNest

**Đọc truyện tranh và sách ngay trên máy chơi game cầm tay.**

[Tiếng Việt](README.vi.md) · [English guide](docs/USER_GUIDE.md) · [Hướng dẫn sử dụng](docs/HUONG_DAN_SU_DUNG.md) · [Cài đặt](docs/CAI_DAT.md)

NXT Retro BookNest brings your comics, novels and books together on a retro handheld. Read from the SD card or an online source, turn the device to your preferred reading direction, and pick up where you left off.

**Version:** 1.0.2 · **Project:** NXT Retro / [SpringThong](https://github.com/SpringThong)

## Download

Installer ZIPs will be attached by the author in **[Releases](https://github.com/SpringThong/NXT-Retro-BookNest/releases)**. If no matching ZIP is listed yet, the installer has not been uploaded there.

| Device | Firmware | Package to choose |
| --- | --- | --- |
| TrimUI Brick Pro | Stock | `NXT_Retro_BookNest_v1.0.2_BrickPro_Stock.zip` |
| TrimUI Brick Pro | NX Redux | `NXT_Retro_BookNest_v1.0.2_BrickPro_NXRedux.zip` |
| TrimUI Brick Pro | NextUI | `NXT_Retro_BookNest_v1.0.2_BrickPro_NextUI.zip` |
| TrimUI Brick Pro | Knulli | `NXT_Retro_BookNest_v1.0.2_BrickPro_Knulli.zip` |
| TrimUI Brick Pro | muOS | `NXT_Retro_BookNest_v1.0.2_BrickPro_MuOS.zip` |
| R36S | DarkOS / dArkOS | `NXT_Retro_BookNest_v1.0.2_R36S_DarkOS.zip` |

Choose **one ZIP matching your device and firmware**. GitHub's automatic “Source code” downloads contain this documentation repository, not the app installer.

## What you can do

| Area | Features |
| --- | --- |
| Offline reading | Browse folders, image collections, CBZ/ZIP comics, TXT, EPUB, supported MOBI/PRC books and PDFs. |
| Online reading | Add a source URL or choose an in-app suggestion; browse categories, search books, open chapter lists and continue to the next chapter when the source provides it. |
| Book layouts | Choose one page, two pages or continuous scrolling, with covers, contents and page-turn effects for supported text formats. |
| Reading comfort | Adjust font, text size, line spacing, margins, contrast, paper/background and text colour; choose light, dark or monochrome reading themes. |
| Navigation | Rotate the reading view, zoom, use manual or automatic scrolling, change scroll speed while reading and configure right-stick zoom. |
| Your library | Resume reading, save bookmarks, search for a chapter and reopen the chapter list from a book in your library. |
| Languages | Vietnamese and English interface, with bundled multilingual font fallback. |
| Performance | Configurable 5–10-page lookahead, default 8; cached rendering and progressive text pagination. Target 60 Hz or choose 30 Hz in Settings. |

The packages share the reading features and interface. Launchers, artwork registration, display output and input handling are adapted to each firmware; R36S displays the interface at 640×480.

## Quick start

1. Download the ZIP for your device and firmware.
2. Follow the [installation table](docs/INSTALLATION.md), then launch BookNest from Apps, Tools, Applications or Ports.
3. For offline reading, open **Downloads / Offline** and browse to your book. For online reading, open **Web sources** and add a source first.
4. Press **START** while reading for chapter selection, fonts, appearance and scrolling controls.

Read the [English user guide](docs/USER_GUIDE.md) or [hướng dẫn tiếng Việt](docs/HUONG_DAN_SU_DUNG.md) for the full controls.

## Default controls

| Button | While reading |
| --- | --- |
| A / SELECT tap | Show or hide the toolbar |
| B | Save position and go back |
| L1 / R1 | Previous / next page |
| L2 / R2 | Zoom an image or change text size |
| R3 click | Rotate the reading view |
| L3 click | Toggle automatic scrolling |
| D-pad / left stick | Navigate or pan, depending on reading mode |
| X | Open text-layout selection, or switch image fit |
| Y | Bookmark the current position |
| START | Open the reading menu |
| SELECT + L2 / R2 | Decrease / increase automatic-scroll speed |
| SELECT + L1 / R1 | Previous / next online chapter when available |
| SELECT + X | Open chapter / contents selection |

In menus, **A confirms and B goes back**. In the text-layout chooser, select your option first, then press **A** to apply. Controls can be remapped in Settings.

## Compatibility notes

- MOBI support covers unprotected MOBI 6/7 and PalmDOC/PRC. KF8-only/AZW3 and DRM-protected books are not supported.
- PDF can use original pages or reflow selectable text. Scanned PDFs stay as images unless they already contain a usable text layer; BookNest does not perform OCR.
- Websites may change domains, page structures or access rules. Source availability and next-chapter navigation depend on what the source exposes.
- Target refresh rate is not a guarantee of measured hardware FPS. NX Redux has received positive user feedback; the other firmware packages have been built and checked automatically but still need device testing. Hardware GPU behaviour and temperatures have not been verified across all six configurations.

## Guides and feedback

- [Vietnamese introduction](README.vi.md)
- [Installation — English](docs/INSTALLATION.md) · [Cài đặt — Tiếng Việt](docs/CAI_DAT.md)
- [User guide — English](docs/USER_GUIDE.md) · [Hướng dẫn sử dụng — Tiếng Việt](docs/HUONG_DAN_SU_DUNG.md)
- [Version 1.0.2 changes](CHANGELOG.md)
- [Report a problem](https://github.com/SpringThong/NXT-Retro-BookNest/issues)

When reporting a problem, include your device, firmware version, BookNest version and steps to reproduce. Logs are `data/launch.log` and `data/BookNest.log` inside the app folder. Remove personal URLs or information before posting logs publicly.

This repository contains the project introduction and user documentation. Component licence notices are included with the app packages.
