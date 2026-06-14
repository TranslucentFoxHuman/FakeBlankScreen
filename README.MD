# FakeBlankScreen  

This app shows the black screen when it starts, and prevents the device from sleeping by acquiring the screen wake-lock. It is intended for devices that have an OLED display.

Do you own a device with an OLED screen and run a long-running background task on it?  
And, do you want that task to keep running while minimizing battery use and avoiding screen burn-in?  
This app is perfect for that situation!

By keeping the screen black, processing in the background is not stopped/restricted unlike putting the device to sleep,
Unlike simply keeping the screen on, it also does not cause OLED burn-in.

## How to Use  
When you launch this app, the black screen will appear.
This app will enable the screen's wake-lock and prevent the device from entering sleep mode. That's all.

To close this app, swipe from the top or bottom edge of the screen to reveal the navigation bar, tap the square button to open the recent-apps list, and close this app from it. This app doesn't have exit function itself.

## Tips  

### I need to move away from my phone while using this app, but I want to keep it secure. What should I do?  
Use Android's [App Pinning](https://support.google.com/android/answer/9455138) feature. Pinning the app blocks opening the notification shade, closing the app, or switching to another app. If someone tries to switch applications, authentication is required, so you can leave the phone safely.

### Can it be used on LCD screens?  
It will run, but it is not useful. With OLED, a black screen consumes zero power, but with LCD the backlight stays on, so power consumption remains still high. It may only help spot dead pixels or backlight blemishes on LCDs.

### Why is the version 2.x.x instead of 1.x.x?  
Version 1.x actually existed (see commit 5a1e3fa0b3fb7660e838ab5fd44fc92d27fde742).  
However, it was developed only for the author's use and did not work on Android versions before 13. And it was created in 2022 so it's very old. Because this app is simple, rewriting it from scratch as a new project was better than trying to improve the old code. The old project files were removed and this app was rewritten completely. The code is no longer compatible with 1.x, so the version was bumped to 2.x.x.

## License
This program is provided under the terms of MIT license.   
In version 1.x, it was GNU GPL v3.