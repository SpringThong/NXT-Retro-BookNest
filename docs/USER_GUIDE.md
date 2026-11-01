# NXT Retro BookNest 1.0.2 user guide

[Overview](../README.md) · [Installation](INSTALLATION.md) · [Tiếng Việt](HUONG_DAN_SU_DUNG.md)

## Library and navigation

Use the D-pad or left stick to navigate, A to confirm and B to go back. The library remembers books you have opened. Select a book to resume; X on a library item opens its chapter list, contents or page selection. Controls can be remapped in Settings.

## Offline reading

Copy books or image folders to the SD card. Open **Downloads / Offline** and browse to the file; Y opens the Books shortcut selected by the firmware launcher.

| Content | Supported formats |
| --- | --- |
| Comics | JPEG, PNG, WebP, image folders, CBZ/ZIP |
| Text and books | UTF-8 TXT, EPUB, unprotected MOBI 6/7 and PalmDOC/PRC |
| PDF | Original pages or reflow of a suitable text layer |

EPUB/MOBI can show covers, titles, authors and contents supplied by the file. EPUB is laid out by the reader and may not reproduce every publisher style. KF8-only/AZW3 and DRM-protected books are not supported.

## Online reading

Connect the firmware to the internet first. A fresh installation starts with an empty source list. In **Web sources**, choose the suggested-source discovery page or press X to enter a URL. Follow the check/confirmation screen, then browse a category or search for a book and choose a chapter.

Comics and novels use the same source-browsing flow. Rankings, categories and other sections depend on what the website provides. In category/contents grids, up/down follows the column and left/right follows the row.

When a next-chapter link is available, you can move to the next chapter without leaving the reader. Use R1 at the end when offered, or SELECT+L1/R1 for chapter navigation. Source availability and complete chapter indexes are not guaranteed.

## Default reading controls

| Button | Action |
| --- | --- |
| L1 / R1 | Previous / next page |
| D-pad / left stick | Navigate, scroll or pan according to the mode |
| L2 / R2 | Zoom images or decrease/increase text size |
| R3 click | Rotate through 0°, 90°, 180°, 270° |
| L3 click | Toggle automatic scrolling |
| A / SELECT tap | Show or hide the toolbar |
| START | Reading menu |
| X | Text-layout chooser, or image fit toggle |
| Y | Bookmark position |
| B | Save position and go back |
| SELECT + L2 / R2 | Decrease / increase automatic-scroll speed |
| SELECT + L1 / R1 | Previous / next online chapter when available |
| SELECT + X | Chapter / contents selection |

Clicking R3 rotates the view. Tilting the right stick is a separate configurable zoom action. Power and sleep remain controlled by the firmware.

## Page layouts and appearance

For supported text books and online chapters, X opens one-page, two-page and continuous-scroll choices. Move to an option, then press **A to apply**; B cancels. Moving the selection alone does not apply it. Page-turn effects can be toggled in the START menu.

Interface and reading fonts are configured separately; the defaults are Quicksand and Literata. L2/R2 changes reading size. The appearance section of the START menu provides paper/light/dark/monochrome themes, text/background colours, line spacing, margins and contrast.

Monochrome is an LCD display theme, not an e-ink screen mode. Bundled fallback fonts cover several scripts, but unusual characters or PDFs with missing Unicode mappings can still need original-page viewing. While a book is being paginated, the total page count may temporarily show `…`.

## Automatic scrolling

L3 toggles automatic scrolling. Change speed in the reading menu or with **SELECT+L2/R2** while reading: 0.25×–4.00×, in 0.25× steps. The reading direction follows rotation. Scrolling stops at a chapter boundary so you can choose the next chapter.

## Right-stick zoom

Settings provides Off, Step and Smooth modes, plus a scope of Comics, Text or Both. The chooser shows the scope shortcut; A saves and B cancels. Comics is the default scope to reduce accidental text-size changes. Enabling text zoom lets stick tilt change font size; R3 click still rotates.

## Chapters, contents and resuming

Use START's chapter-selection entry or SELECT+X while reading. In the chapter list, START searches by chapter number or part of its title. Online indexes may continue loading in the background, and some sources have missing chapters.

EPUB contents come from the book; TXT recognises some chapter-heading patterns. Page selection remains available when a suitable contents list is absent. B leaves the reader and saves your position.

## PDFs

Automatic classification chooses between text reflow and original pages. Text PDFs can be reflowed for font and size changes; image/scanned or mixed PDFs normally retain their original pages.

In **START → PDF**, cycle through **Auto → Original pages → Reflow text**. Choose manually if automatic detection is unsuitable. Complex columns, tables and missing Unicode mappings may reflow poorly; original pages retain the printed layout.

BookNest does not perform OCR. Password-protected PDFs must be legitimately unlocked before use. Version 1.0.2 limits: 512 MiB per PDF, 2,000 pages and 8 MiB extracted text. Original-page rasters are capped at 1024×1536; deep zoom does not automatically rerender them at higher resolution.

## Source changes and timeouts

Select a saved source in Web sources and press R2 to change its URL. Enter the new address, press START to check it and A to confirm. The app retains the source ID and migrates same-host links where applicable.

A domain change may be handled this way. Changes to page structure, book/chapter paths or APIs may need a new reader adapter or a fresh book lookup. The app does not log in to websites or bypass their verification.

For timeouts, check firmware connectivity, retry and verify the website address. A 403/CDN refusal does not by itself mean your local data is damaged. Downloads in `data/books` remain separate from disposable cache.

## Settings, performance and support

Settings includes Vietnamese/English, key mapping, fonts, 5–10-page lookahead (default 8), 30/60 Hz update target and stick-zoom options. Large images can reduce the number of decoded pages held in RAM. Actual performance varies by file, website, storage, hardware and firmware; identical FPS or temperature across devices is not guaranteed.

Back up the app's `data` folder and keep it during updates. For an issue, include the device, firmware version, app version, format, reproduction steps and relevant logs: `data/launch.log` and `data/BookNest.log`. Remove personal paths, URLs and unrelated information before posting publicly. Share only sample content you are allowed to distribute.
