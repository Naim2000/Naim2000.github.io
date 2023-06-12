# Region changing an MKW save file

## Requirements
- Dolphin Emulator 
  - You don't need a beefy PC, you aren't going to run the game.
- an SD card
- The Homebrew Channel

## Instructions

### Section I: Extracting your save file
- If you have always used `Save to SD Card`, skip this section, you can find rksys.dat in `sd:/riivolution/save/RMCx/`.
  - `x` is the region letter of the game, E = NTSC-U, J = NTSC-J, P = PAL, K = Korea
- If you are converting the save file *for* Dolphin Emulator, skip this section, you can find rksys.dat in `nand/tite/00010004/524d43xx/data/`.
  - `nand` is the path in `Config > Paths > Wii NAND Root`.
  - `xx` is the region letter of the game in hex. 45 = E (NTSC-U), 4a = J (NTSC-J), 50 = P (PAL), 4b = K (Korea)
- You may also create a NAND backup and import it into Dolphin via `Tools > Manage NAND... > Import BootMii NAND Backup`.

1. Use SaveGame Manager GX (<https://oscwii.org/library/app/savegame_manager_gx>) to copy your save file to your SD. It should appear in `sd:/savegames/RMCx.bin`.
  - If you have Priiloader's `Disable NoCopy Save File Protection` hack enabled, you may copy the save through Data Management. Your save will be found in sd:/private/wii/RMCx/data.bin`.
1. Import it into Dolphin Emulator via `Tools > Import Wii Save`.
1. Open `Config > Paths` and open the path listed under Wii NAND Root in a File explorer window.
1. Navigate to `title > 00010004 > 524d43xx`, and make a copy of the folder.
1. Remove the (copy) from the name and change the last 2 letters to the desired region (see notes above)

### Section II: Converting rksys.dat

1. Go to https://www.tt-rec.com/ghostmanager.
1. Upload your rksys.dat
1. Scroll down to the Download button. Click the dropdown to the right of it and select your region to your desired region (US, EU, JP, KR?), then press the Download button itself.
1. Save the file to the same place you uploaded it (replace it).
  - If you are converting the save file for Dolphin Emulator, you may opt to make a backup of the original rksys.dat

### Section III: Importing the new save
- If you are converting the save for Dolphin Emulator, gg you're done.

1. Select `Tools > Export All Wii Saves`.
1. Select your SD card.
1. Put your SD card back into your Wii, and copy the save through Data Management.
