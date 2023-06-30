# Region changing an MKW save file

## Prerequisites
- [Dolphin Emulator](https://dolphin-emu.org/download)
- an SD card
- The Homebrew Channel
- [SaveGame Manager GX](https://oscwii.org/library/app/savegame_manager_gx)

## Instructions

### Section I: Extracting your save file (rksys.dat)
1. Download and extract SaveGame Manager GX to your SD card, and launch it from the Homebrew Channel.
1. Select your Mario kart Wii save, and click `Extract`, and select `Default`.
1. Exit SaveGame Manager GX, and put your SD card into your PC.
1. Open Dolphin Emulator and select `Tools > Import Wii Save`.
1. Open your SD card and select `savegames > RMCX.bin` (`X` is a placeholder!)
1. Select `Config > Paths` and open the path listed under `Wii NAND Root`.
1. Find `title > 00010004 > 524d43xx` and change the last 2 letters to the desired region:
  - USA: `45`
  - EUR: `50`
  - JPN: `4a`
  - KOR: `4b`

Your `rksys.dat` will be found in the `data` folder.

### Section II: Converting rksys.dat

1. Go to <https://www.tt-rec.com/ghostmanager>.
1. Upload your `rksys.dat` file.
1. Click the dropdown at the bottom right and select your desired region.
1. Press the Save & Download button.
1. Save the file to the same place you uploaded it (replace it!)

### Section III: Importing the new save

1. Select `Tools > Export All Wii Saves`.
1. Select your SD card.
1. Eject your SD card, then put it back into your Wii.
1. Go to `Data Management > Save Data > Wii > SD Card` and copy over the Mario kart Wii save file.
