# Mainichi Issho Portable(Everyday Together) Revival server. 
This is a mainichi issho patch that will allow you to connect to revival servers! Right now there are only 3 episodes available to watch which are dumped from the Trial version of mainichi issho, if you played this on a PS3 or PSP back when it was still allive please share your savedata and game dumps! As they would help in restoring the contents. Also you are required to patch a few syscalls.

# Tutorial on how to patch the game
Requrements:
- A Laptop or pc
- PPSSPP (Latest Version)
- Copy of Mainichi issho Portable(ISO or PKG)
- An extractor, for PKG use PSNPKGDecryptor&Extractor for ISO you can mount it and copy files from there or using winrar
- attention(yes, pls pay very much attention)

## Tutorial
### Step 1
Unpack your copy of mainichi issho using the tools above into a folder.
### Step 2
Download The MAIN.KSC file from this repo
### Step 3
Open your folder with mainichi issho and navigate to PSP_GAME then USRDIR folder.
### Step 4
Copy over the MAIN.KSC file and overwrite the existing file.
### Step 5
Launch PPSSPP and navigate to the directory where you unpacked your install and launch it.
### Step 6
Open Debug menu on top of the ppsspp window and click Break This will stop the game this is needed for a short time then open Debug menu again on top of the ppsspp window and open Disassembly and click on a random line so it will get blue(selected).
Once in there press Ctrl+F or if youre on a Mac Command+F then type in sceNpAuthGetEntitlementIdList.
You will see a bunch of lines and the one you need is the one that was found with that address right click it and press Assemble Opcode and type in "nop" click okay and repeat the same process until there isnt any sceNpAuthGetEntitlementIdList. After that close disassembly window then open debug menu and hit Run.
### Step 7
After Everything is done head to the update menu and click it and select the first option that appears <img width="944" height="528" alt="image" src="https://github.com/user-attachments/assets/9f2fdcba-5cbc-416b-94aa-9b07021dd14d" />
It will then get stuck and it will be frozen thats fine click Debug on top of ppsspp window then Click break then open Disassembly click on a random line press Ctrl+F or for Mac Command+f and type sceNpAuthGetEntitlementById then under the line that was found there should be a line with "bgelz" in it right click on it and click on Assemble Opcode and type "nop"
then close Disassembly click on Debug on top the Window and Press Run wait a bit and you're done!
### Step 8
After that you should complete setting it up and finally get to the main menu, click on Update button located at the very bottom of the menu.
### Step 9
Wait for it to finish downloading everything and you're done! If it throws an error retry a few times or restart PPSSPP,  make sure you also have infrastructure and WLAN turned on in ppsspp and that you have a stable internet connection.
