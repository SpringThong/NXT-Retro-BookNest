# Install NXT Retro BookNest 1.0.2

[Overview](../README.md) · [User guide](USER_GUIDE.md) · [Tiếng Việt](CAI_DAT.md)

## Pick the matching package

Installers will be attached in [Releases](https://github.com/SpringThong/NXT-Retro-BookNest/releases). Choose the ZIP for the installed firmware.

| Device / firmware | Extract into | Expected entry | Launch from |
| --- | --- | --- | --- |
| Brick Pro / Stock | SD-card root | `Apps/NXT_Retro_BookNest/launch.sh` | Apps |
| Brick Pro / NX Redux | SD-card root | `Tools/NXT_Retro_BookNest.pak/launch.sh` | Tools |
| Brick Pro / NextUI | SD-card root | `Tools/tg5040/NXT_Retro_BookNest.pak/launch.sh` | Tools |
| Brick Pro / Knulli | SHARE root, corresponding to `/userdata` | `roms/ports/NXT_Retro_BookNest.sh` | Ports |
| Brick Pro / muOS | Root of the card holding MUOS | `MUOS/application/NXT_Retro_BookNest/mux_launch.sh` | Applications |
| R36S / DarkOS | EASYROMS root on the active ROM card | `ports/NXT_Retro_BookNest.sh` | Ports |

Preserve the ZIP's folder structure. Keep the Stock folder name with underscores; do not replace them with spaces.

## First installation

1. Exit any running app before replacing files or removing the card.
2. Extract the matching installer to the location above.
3. Copy the complete app folder, including fonts, the PDF runtime and support files.
4. Reinsert the card and launch BookNest. Refresh the Ports list if the new entry is missing.

No Python or PortMaster installation is needed. Knulli, muOS and DarkOS packages use the firmware's AArch64 SDL2. The private PDF reader runtime is included.

## Updates and saved data

Exit BookNest and replace the app files with the complete new package. **Keep the existing `data` folder** to preserve sources, reading history, bookmarks, settings and downloads. Installer ZIPs do not contain personal data.

When moving between firmware, back up `data` first and check book paths after the move; mount paths may change. Keep the old copy until the new installation can read your books.

## Offline books

Stock/NX Redux/NextUI use a shortcut to `Books` at the SD-card root. Knulli and DarkOS resolve storage from their installation location; DarkOS does not lock the app to `/roms` or `/roms2`. muOS uses the firmware's configured storage when its setup helpers are available. In-app downloads remain under `data/books`.

Open **Downloads / Offline** and press **Y** to open the Books shortcut. You can also browse another folder.

## Launcher artwork

Stock has its app configuration and icon images. NX Redux retains its recognised-launcher logo repair. NextUI includes `.media` artwork; enable Game Art to show it when selecting BookNest. muOS includes an application glyph.

Knulli/DarkOS register the BookNest entry in the Ports gamelist on first launch. Exit and refresh the game list to load the artwork. Other entries and metadata are retained. Settings provides app-icon repair; malformed or unwritable gamelists are kept and the reason is logged.

## If the app does not start

Check the device/firmware package, folder structure and complete file copy. On Stock, check the folder name for spaces. Logs are `data/launch.log` and `data/BookNest.log` inside the app folder. Include the firmware version and reproduction steps in a report; keep your data while troubleshooting.
