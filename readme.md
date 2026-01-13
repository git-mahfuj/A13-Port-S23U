# Samsung A13 – Flash ONEUI-7 (FastbootD Method)

⚠️ WARNING
Wrong file or wrong order = HARD BRICK
Only for BOOTLOADER UNLOCKED devices.

--------------------------------------------------

REQUIREMENTS
- Bootloader Unlocked
- OEM Unlock ON
- ADB & Fastboot installed
- Custom Recovery (GIVEN IN REPO)
- super.img
- boot.img
- vbmeta.img.tar
- Odin
- Battery 60%+
- Download the necessary files here:  
[https://drive.google.com/file/d/1bmdgYlJ6m72yEwFzt2FRbl1-f_cZEeNl/view?usp=drive_link](https://drive.google.com/file/d/1bmdgYlJ6m72yEwFzt2FRbl1-f_cZEeNl/view?usp=drive_link)


--------------------------------------------------

STEP 1: Flash Recovery via Odin
1. Boot phone into Download Mode
2. Open Odin
3. AP → select recovery.img.tar
4. Auto Reboot = OFF
5. Click Start
6. Flash complete then
   Force reboot directly into Recovery
   (Power + Volume UP)

--------------------------------------------------

STEP 2: Enter FastbootD
Recovery menu:
Advanced → Enter FastbootD

--------------------------------------------------

STEP 3: Flash Images via FastbootD (PC)
Connect usb then type the command in terminal/powershell:

- fastboot devices

- fastboot erase userdata
- fastboot erase cache

- fastboot flash super super.img
 (Take 2–5 minutes, Don't Interrupt)

- fastboot flash boot boot.img

- fastboot reboot

--------------------------------------------------

STEP 4: Flash vbmeta (MANDATORY)
Reboot Phone then Download Mode (Mandatory)

Odin:
AP → vbmeta.img.tar
Click Start

If you won't flash vbmeta :
- Bootloop
- Red State Error
- Verified Boot Failure

STEP 5 : FACTORY RESET
- Reboot Phone to recovery then factory reset
- Reboot to system

--------------------------------------------------

Congrats: First Boot
- First boot take 5–10 minutes 
- Don't Panic if fail go to DownloadMode then Flash stock rom

--------------------------------------------------

BUGS
- Recent Apps Section in Black
- FingerPrint don't work

--------------------------------------------------

Try it 😜 
