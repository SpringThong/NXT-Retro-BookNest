# Changelog

## 1.0.2

### Responsiveness

- Text pagination continues in small portions, including inside long paragraphs; the requested reading spread is prioritised over the complete page index.
- Font-size changes keep the latest request and no longer require a synchronous whole-book layout before opening a menu or rotating.
- Stable-scale image panning reuses the existing viewport and samples newly exposed regions.
- Cached rendering, ARM64 framebuffer output, bounded caches and background state writes reduce work in the interaction path.
- Distant prefetch yields to recent input; idle work is reduced. Lookahead remains configurable from 5 to 10 pages, default 8.

### Firmware packages

- TrimUI Brick Pro: Stock, NX Redux, NextUI, Knulli and muOS.
- R36S: DarkOS / dArkOS.
- Shared reader features with firmware-specific launchers, display/input integration and artwork registration.
- SDL2 output for Knulli/muOS/DarkOS fits the logical interface to the display; R36S uses 640×480.
- PDF worker environment is isolated from frontend library/preload overrides.

### Reading features included

Online/offline comics and text, EPUB/MOBI/PDF support within documented limits, covers and contents, chapter search/navigation, bookmarks and resume, one/two-page or scrolling layouts, rotation, configurable stick zoom, appearance settings, automatic scrolling and Vietnamese/English UI.

### Validation

The multi-ROM build passed 171 test cases for the framebuffer configuration and 173 for the SDL2 configuration, including subtests. ARM64/QEMU checks covered SDL2 output/input, framebuffer mapping and the native PDF worker. All six app executables were reproduced byte-for-byte from their corresponding build inputs.

These checks do not establish physical-device GPU behaviour, sustained FPS or temperature on every ROM. NX Redux has received positive user feedback; other device/firmware combinations still require real-device validation.
