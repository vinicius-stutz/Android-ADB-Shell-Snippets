# Android-ADB-Shell-Snippets
ADB Shell Snippets for Android Devices

## Enable Developer options on your smartphone
1. Go to Settings > About phone > Software information.
2. Tap on Build number 7 times (until you get the ‘You’re now a developer!’ message).

## Enable USB Debugging via the Developer options
1. Go to Settings > Developer options > Toggle on USB debugging.
2. Now, head over to your computer and download the ADB tools. [Download the SDK Platform Tools](https://developer.android.com/studio/releases/platform-tools.html) (Windows, Linux, and Mac).
3. Once you’ve downloaded the SDK Platform Tools, simply extract the tools to a convenient location on your PC.
4. Proceed by connecting your device to your PC via a USB cable.
	1. Make sure the USB connection is set to **Transferring files**.
	2.  This can be done via the notification tray itself.
5. Now head over to the **SDK Tools** folder you extracted in **step 3**.
	1. Left Click on the empty space in the SDK folder. Press Shift+Right Click to bring a menu and select **Open command prompt here**. (if you see the option **Open Powershell window here**, select it as this will do, too.)
	2.  Alternatively, simply type cmd in the address bar and hit the Enter key to open a command window right there.
6.  Enter the command `adb devices` just to make sure your smartphone is recognized. You will get a random serial number if ADB is working.

## Enable Android 10 gesture navigation on third-party launchers
```
adb shell cmd overlay enable com.android.internal.systemui.navbar.gestural
```
