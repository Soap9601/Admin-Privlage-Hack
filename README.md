# Admin-Privlage-Hack

his is the fastest way you can get admin rights at work,school,etc in only a few steps :)

First, you need to create a Windows install USB. You have 2 ways: create a bootable Windows 10 USB with the media creation tool

OR

Search on the internet a .iso file of Windows 10 and flash it with using RUFUS.

after that, simply open the USB's directory and put all these files in the ROOT folder. there are a few steps to follow in order to do this trick, but it's really simple, follow me :) P.S. you can also execute the commands one-by-one but this may take much more time than these simple files to execute.

plug the usb into the target pc and enter the BIOS, you can use the f2 f8 f10 f11 ecc combinations, or you can just reboot your pc normally, but keeping pressed the SHIFT key when clicking on "reboot" to boot into the "problem solving" screen where you have to press on it and press on the button to open the BIOS/UEFI settings.

go to the boot section and put your USB in the upper position, then save and exit. (or you can just use "boot override" if you don't want to change boot order)

once you booted into your USB, you should see the "Windows Installer Window". Press SHIFT + F10 to bring up the cmd.

find your USB drive letter, so try the alphabet until you enter the USB.

found the drive letter of the coolest usb ever? confirm it with the "dir" command to get a list of the files inside of it. Now execute the all-in-one script "adminexploit.bat" (yes, it's a .bat so you can actually see and edit what it does.)

press 1 and enter for the first step. It does a bunch of stuff, it just covers your ass in case something goes wrong, no worries. When it's done, PRESS ANY KEY, wait for the timer to end and before your pc reboots, remove the usb.

when the login screen appears, press any key and click on the small accessibility icon to open the cmd you just created.

Cmd should appear. Reconnect and get into the usb again, same as step 4 (If it doesn't, it's because Windows Defender detected it. You can't do anything about it other than trying to find a way to disable it. BASICALLY YOU CAN'T CONTINUE, TRY ANOTHER METHOD. (I'll post an update if I'll a way to do it without admin privileges)

execute adminexploit.bat again and this time press 2. Two windows should appear, one is the cmd where you have to type the commands manually because windows sucks and doesn't let them run automatically ,and the other one is a simple text file from which you have to copy those two commands, adding the name and password you want where they need to be set and then adding (with the second command) the account you just created to the "Administrators" localgroup.

If everything went correctly, you should have the cmd saying "press a key to continue" and then it closes by itself. Cool, but you're not done yet.

now, in the cmd left open, execute "taskkill /F /IM LogonUI.exe" or you can just reboot the pc. This will reload the login screen and hide every window opened.

Perfect! You should see in the bottom left corner the username you created in 2! Click on it and type in your beautiful password.

P.S. If you're on a domain pc, like at school or work there the accounts are managed by a server you have to type this in order to login with a LOCAL ACCOUNT:

"[DOT][BACKSLASH][USERNAME]" (without quotation marks) as user and your password. Example: if the user account is admin, use ".\admin" as username.

DONE! Check if you have admin privileges by pressing on start > account icon > change account settings. If it says Local Account - Administrator, you are now admin!

The last thing you have to do is execute for the last time the adminexploit.bat script and select the 3rd option to restore the original Utilman.

[OPTIONAL FROM HERE ON] HERE COMES THE PROBLEMS: Sometimes with the newer version of windows the 3rd script does not work, resulting in the cmd.exe with the name of Utilman.exe not being replaced with the original Utilman.exe. In this situation, if you want to restore it you have to do some manual steps I can't automate, but I can guide you thrugh them.

Boot into the usb (I swear it's the last time you have to do it). .

Click NEXT

Then click on the bottom left text saying something like "reset the computer"

Then click on Throubleshoot

Then click on System Image Recovery and, if needed, select windows 10 .

Click cancel, next, Advanced, Install a driver, OK.

Now in this explorer window you can access all files. You have to go into your usb root, copy the original Utilman.exe I provided in the repo and paste it into C:\Windows\System32 folder. Delete/overwrite the current one if needed.

Now close everything and reboot the system. I hope this way restores everything back to normal.

YOU DID IT. CONGRATS. NOW DON'T GET CAUGHT USING YOUR NEW ACCOUNT AND REMEMBER TO LOGOUT AND LOGIN INTO A NORMAL ACCOUNT BEFORE LEAVING.

Thank us later with a STAR on GitHub, it would make us proud of our work :)
