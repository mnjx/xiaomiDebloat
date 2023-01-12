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
6. Paste the *CODE* into the command prompt (*without the `CODE START` and `CODE END`*)
7. Once it says `DONE`, you can close the command prompt.
8. You should now have a debloated Xiaomi phone.

`CODE START `

`adb shell `

`pm uninstall -k --user 0 com.miui.msa.global `

`pm uninstall -k --user 0 com.xiaomi.glgm `

`pm uninstall -k --user 0 com.facebook.appmanager `

`pm uninstall -k --user 0 com.facebook.services `

`pm uninstall -k --user 0 com.facebook.system `

`pm uninstall -k --user 0 com.mi.webkit.core `

`pm uninstall -k --user 0 com.android.calendar `

`pm uninstall -k --user 0 com.miui.calculator `

`pm uninstall -k --user 0 com.android.deskclock `

`pm uninstall -k --user 0 com.android.mms `

`pm uninstall -k --user 0 com.miui.smsextra `

`pm uninstall -k --user 0 com.miui.screenrecorder `

`pm uninstall -k --user 0 com.miui.cleanmaster pm uninstall -k --user 0 com.miui.fm `

`pm uninstall -k --user 0 com.mi.android.globalFileexplorer `

`pm uninstall -k --user 0 com.mi.android.globalpersonalassistant `

`pm uninstall -k --user 0 com.miui.fmservice `

`pm uninstall -k --user 0 com.milink.service `

`pm uninstall -k --user 0 com.miui.videoplayer `

`pm uninstall -k --user 0 com.miui.yellowpage `

`pm uninstall -k --user 0 com.mipay.wallet.in `

`pm uninstall -k --user 0 com.mipay.wallet.id `

`pm uninstall -k --user 0 com.xiaomi.payment `

`pm uninstall -k --user 0 com.android.browser `

`pm uninstall -k --user 0 com.miui.hybrid `

`pm uninstall -k --user 0 com.miui.android.fashiongallery `

`pm uninstall -k --user 0 com.miui.player `

`pm uninstall -k --user 0 com.miui.translation.kingsoft `

`pm uninstall -k --user 0 com.miui.translationservice `

`pm uninstall -k --user 0 com.miui.virtualsim pm uninstall -k --user 0 com.miui.compass `

`pm uninstall -k --user 0 com.duokan.phone.remotecontroller `

`pm uninstall -k --user 0 com.miui.bugreport `

`pm uninstall -k --user 0 com.miui.translation.youdao `

`pm uninstall -k --user 0 com.xiaomi.joyose `

`pm uninstall -k --user 0 com.miui.notes `

`pm uninstall -k --user 0 com.xiaomi.mipicks `

`pm uninstall -k --user 0 com.xiaomi.scanner `

`pm uninstall -k --user 0 com.xiaomi.midrop `

`pm uninstall -k --user 0 com.miui.hybrid.accessory `

`pm uninstall -k --user 0 com.miui.daemon `

`pm uninstall -k --user 0 com.miui.analytics `

`pm uninstall -k --user 0 com.caf.fmradio `

`pm uninstall -k --user 0 com.miui.cloudservice `

`pm uninstall -k --user 0 com.miui.cloudservice.sysbase `

`pm uninstall -k --user 0 com.miui.cloudbackup `

`pm uninstall -k --user 0 com.miui.backup `

`pm uninstall -k --user 0 com.miui.micloudsync `

`pm uninstall -k --user 0 com.miui.miservice `

`pm uninstall -k --user 0 com.xiaomi.micloud.sdk `

`pm uninstall -k --user 0 com.miui.gallery `

`pm uninstall -k --user 0 com.miui.vsimcore `

`pm uninstall -k --user 0 com.miui.weather2 `

`pm uninstall -k --user 0 com.netflix.partner.activation `

`pm uninstall -k --user 0 com.miui.wmsvc `

`pm uninstall -k --user 0 com.google.android.youtube `

`pm uninstall -k --user 0 com.google.android.apps.maps `

`pm uninstall -k --user 0 com.android.chrome `

`pm uninstall -k --user 0 com.google.android.music `

`pm uninstall -k --user 0 com.google.android.apps.docs `

`pm uninstall -k --user 0 com.google.android.videos `

`pm uninstall -k --user 0 com.google.android.apps.photos `

`pm uninstall -k --user 0 com.android.stk `

`pm uninstall -k --user 0 com.android.cellbroadcastreceiver `

`pm uninstall -k --user 0 com.google.android.tts `

`pm uninstall -k --user 0 com.google.android.marvin.talkback `

`pm uninstall -k --user 0 com.android.bookmarkprovider `

`pm uninstall -k --user 0 com.android.dreams.phototable `

`pm uninstall -k --user 0 com.android.dreams.basic `

`pm uninstall -k --user 0 com.android.wallpaper.livepicker `

`pm uninstall -k --user 0 com.android.bips `

`pm uninstall -k --user 0 com.android.printspooler `

`pm uninstall -k --user 0 com.google.android.printservice.recommendation `

`pm uninstall -k --user 0 com.android.emergency `

`pm uninstall -k --user 0 com.android.internal.display.cutout.emulation.tall `

`pm uninstall -k --user 0 com.android.internal.display.cutout.emulation.corner `

`pm uninstall -k --user 0 com.android.internal.display.cutout.emulation.double `

`pm uninstall -k --user 0 com.google.android.inputmethod.latin `

`pm uninstall -k --user 0 com.hippogames.ludosaga.mi `

`pm uninstall -k --user 0 com.block.puzzle.game.hippo.mi `

`pm uninstall -k --user 0 com.mi.global.shop `

`pm uninstall -k --user 0 in.amazon.mShop.android.shopping `

`pm uninstall -k --user 0 com.netflix.mediaclient `

`pm uninstall -k --user 0 com.opera.app.news `

`pm uninstall -k --user 0 com.opera.branding `

`pm uninstall -k --user 0 com.opera.branding.news `

`pm uninstall -k --user 0 com.opera.mini.native `

`pm uninstall -k --user 0 com.mi.global.bbs `

`pm uninstall -k --user 0 com.facebook.katana `

`pm uninstall -k --user 0 in.mohalla.brandprovider `

`pm uninstall -k --user 0 in.mohalla.sharechat `

`pm uninstall -k --user 0 com.duokan.phone.remotecontroller.peel.plugin `

`pm uninstall -k --user 0 com.eterno `

`pm uninstall -k --user 0 net.one97.paytm `

`pm uninstall -k --user 0 com.miui.userguide `

`pm uninstall -k --user 0 com.android.thememanager `

`pm uninstall -k --user 0 com.google.android.apps.tachyon `

`pm uninstall -k --user 0 com.google.android.feedback `

`pm uninstall -k --user 0 com.google.android.gm `

`pm uninstall -k --user 0 com.google.android.googlequicksearchbox `

`pm uninstall -k --user 0 com.google.android.syncadapters.calendar `

`pm uninstall -k --user 0 com.google.android.syncadapters.contacts `

`pm uninstall -k --user 0 com.miui.miwallpaper `

`pm uninstall -k --user 0 com.miui.translation.xmcloud `

`pm uninstall -k --user 0 com.miui.touchassistant `

`pm uninstall -k --user 0 com.xiaomi.discover `

`pm uninstall -k --user 0 com.xiaomi.location.fused pm uninstall -k --user 0 com.xiaomi.mirecycle `

`pm uninstall -k --user 0 com.xiaomi.providers.appindex `

`pm uninstall -k --user 0 com.xiaomi.xmsf `

`pm uninstall -k --user 0 com.android.vending `

`pm uninstall -k --user 0 com.google.android.gms `

`pm uninstall -k --user 0 com.xiaomi.finddevice `

`pm uninstall -k --user 0 com.mi.globalbrowser `

`pm uninstall -k --user 0 com.miui.face `

`pm uninstall -k --user 0 com.android.providers.contacts `

`pm uninstall -k --user 0 com.google.mainline.telemetry`

`pm uninstall -k --user 0 com.qualcomm.qti.qms.service.telemetry `

`DONE `
`CODE END`
