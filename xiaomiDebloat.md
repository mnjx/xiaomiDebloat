# How to debloat your Xiaomi phone (MIUI 12 and lower)

## Prerequisites

### ***Windows***

+ **Android USB drivers:** https://developer.android.com/studio/run/win-usb, extract the archive,
  connect your phone to your PC, open Device Manager by right clicking the Windows icon on the taskbar, expand the
  "Portable Devices" section (your phone should be there (if it is not there, just check all the other sections
  and also check the connectivity between your phone and PC and then try again)), right click your phone,
  click "Update driver", click "Browse for drivers in my computer", now you should see
  a "Browse..." button, click it and navigate to your extracted folder with the USB drivers, click "OK", click "Next",
  now your USB drivers should be installed.
+ **ADB tools:** https://developer.android.com/studio/releases/platform-tools, extract the archive.

### ***Phone***

+ **F-Droid and/or Aurora store:** F-Droid: https://f-droid.org/, Aurora store: Get it on F-Droid
+ **A web browser:** I recommend Bromite https://bromite.org, Brave https://brave.com or LibreWolf https://librewolf.net
+ **Simple keyboard app from F-Droid:** Get it on F-Droid
+ **Enable USB debugging:** Go to settings, about phone, and start clicking on the "MIUI Version" button until it shows
  a message that shows "Voilà, you are now a developer!", go back to settings, click on
  "Additional settings", "Developer options" and scroll down until you can see a toggle labeled "USB debugging"
  and toggle it on.
+ *Note that the code below is going to remove some apps, you might not want to be removed, like Android Calendar, but don't worry, since you can install anything later on either from F-Droid or Aurora store.*

## Debloating from a Windows PC:

1. Open the folder containing the ADB tools and left click in the address bar with the path to the folder on the top of the window.
2. Type `cmd.exe` (*this will open command prompt inside that folder*).
3. Into the command prompt type `adb devices`.

   *You should see something like:*

   `List of devices attached`

   `b71ab4796d23    unauthorized`
4. Move over to your phone, and authorize the PC to make changes to the phone (the phone should prompt you).
5. Again type `adb devices`.

   *You should see something like:*

   `List of devices attached`

   `b71ab4796d23    device`
6. Download the "[debloat.bat](https://github.com/mnjx/xiaomiDebloat/blob/main/debloat.bat)" file, move it into the folder containing the ADB tools and execute is as administrator.
7. Once it shows `DONE` in the terminal, you can close the command prompt and disconnect your phone from your PC.
8. You should now have a debloated Xiaomi phone.
