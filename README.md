# Dell S2716DGR Calibration Guide
The goal of this guide is to get better overall image quality from the Dell S2716DG or S2716DGR 27" 2560x1440p 144Hz G-Sync monitor. Out of the box this monitor has a reputation for washed out colors, but when calibrated has a crisp, sharp image with very good color reproduction. The difference from out of the box to calibrated is a night and day change and well worth spending a couple of minutes to tweak. Going forward, I will use the models S2716DG and S2716DGR interchangably. The only difference is one is a retail model, all specs are the same.

### Requirements
- A Dell S2716DG or S2716DGR 27" 2k 144Hz G-Sync Monitor
- A modern Nvidia GPU
- The Nvidia drivers with Nvidia Control Panel installed (I recommend the latest version to support your GPU)
- Ideally a DisplayPort cable to connect your Dell S2716DG/S2716DGR and computer/GPU. G-Sync and 144Hz are only supported via DP by the monitor.
- The Dell S2716DG monitor driver from Dell

### Resources
- [Dell S2716DG manual](https://www.dell.com/support/home/us/en/19/product-support/product/dell-s2716dg-monitor/manuals)
- [Dell S2716DG driver](https://www.dell.com/support/home/us/en/19/product-support/product/dell-s2716dg-monitor/drivers) Be sure to pick the proper OS from the drop down, IE: Windows 10 64-bit, Windows 7 64-bit, etc.
- [Nvidia GeForce drivers](https://www.geforce.com/drivers) Be sure to pick the proper driver for your GPU if you have not installed it already. This should include the Nvidia Control Panel.

### Intro to Calibration
This guide is not meant to be precise. I have not used equipment to measure color accuracy or other aspects of the calibration. Its simply meant to achieve the best overall picture, in my opinion, for using the Dell S2716DGR as it was meant to be used. The monitor is aimed at high performance gaming and I have found these settings to result in no ghosting, a sharp image with very good colors and a balanced brightness good for bright or dark environments.

I will break this guide down into three (3) parts:

1. Installing required software (assumes its downloaded locally already)
2. Calibrating the monitor from the monitor's front panel controls and on screen display (OSD)
3. Calibrating the monitor from the Nvidia Control Panel software

I will assume the monitor is connected properly to the GPU, displays an image from the computer and that all of the resources needed including downloading software is complete. Its also assumed that you have already set the resolution to display (IE: 2560x1440), set the refresh rate (IE: 144Hz) and set your desired G-Sync settings.

Note: I found setting "response time" via the OSD (Display | Response Time) to "fast" to result in very noticable ghosting on the screen and fuzziness with quick movement on the screen. I personaly have this set to "normal" and feel it delivers the best balance of response time and picture quality. Page 11 of the manual states regarding response time "3ms (typical) for Normal mode" and "1ms (typical) for Fast mode". Feel free to try out both modes for yourself.

### Warning
I am not responsible for any steps you take in an attempt to calibrate your monitor. The information provided is done so strickly as is and with not warranty explicit or implied. Should you choose to adjust these settings you do so at your own risk and fully understanding you are responsible for the outcome.

### 1 - Installing Software
#### Nvidia Drivers
For a detailed step-by-step process with screenshots, see the [official Nvidia directions](https://nvidia.custhelp.com/app/answers/detail/a_id/2900/~/installing-nvidia-display-drivers-under-windows-7%2C-windows-8%2C-or-windows-10) for installing the Nvidia GeForce drivers.

Its my experience that you typically do not need to run the installer as an administrator, especially on a home machine that you own. Try it without running as an admin, I would only recommend trying it as an admin if you have issues installing it without.

I would recommend selecting the "Custom (Advanced)" option instead of "Express (Recommended)", and ensure that all the boxes for the listed items are checked, except the "Perform clean install" box. Only use the clean install option if you had a driver from the OEM of the GPU installed or if you have problems installing otherwise.

When complete, I highly recommend rebooting the computer

#### Dell S2716DG Driver
As far as I can tell this driver may not have a major impact on the picture quality but seems to install some sort of color profile. In my subjective opinion, the image looked better with this installed than without. I see no downside to installing the driver.

Simply run the .exe file and follow the steps. Once installed device manager, or in Windows 10 Settings | Devices, should show the monitor as a Dell S2716DG instead of a generic monitor.

A reboot may not be needed, but I would recommend it anyhow.

### 2 - OSD Calibration
These settings are applied directly on the monitor using the front panel (bottom right) physical buttons. The user manual for the Dell S2716DG clearly explain what each button does, but it is pretty intuitive even without that.

I recommend the following settings:
#### Monitor Settings
- Brightness: 75%
- Contrast: 77%

#### Color: Custom Color
- Red (R): 97%
- Green (G): 99%
- Blue (B): 96%

### 3 - Nvidia Control Panel Settings
The Nvidia control panel can be opened by right clicking on the desktop backgroud and selecting Nvidia Control Panel from the context menu. There may also be an Nvidia icon in the notifications area, the bottom right of the screen by the clock on the taskbar, which will open the Nvidia Control Panel.

On the left hand side select "Adjust desktop color settings". On the right, select "Use Nvidia settings". Take note of the "Color channel" drop down, we will be using this to switch to various groups of settings. It should, by default, be set to "All channels".

#### All Channels
- Brightness: +45%
- Contrast: +55%
- Gamma: +0.96
- Digital Vibrance: +45%

#### Red Channel
- Brightness: +40%
- Contrast: +70%
- Gamma: +1.00

#### Grenn Channel
- Brightness: +50%
- Contrast: +50%
- Gamma: +0.89

#### Blue Channel
- Brightness: +50%
- Contrast: +50%
- Gamma: +1.00

### Conclusion
I have found the above to give me the best color and picture quality the Dell S2716DGR has to offer. After calibrating the colors, I have no complaints about the color reproduction or picture. I am really enjoying gaming on the Dell S2716DGR. Hopefully these settings will help others enjoy the S2716DG to its maximum potential.

Feel free to tweak the above settings to your prefence. If you found settings you feel look better than these, open an issue and share them.

### Dell S2716DG and Dell S2716DGR info
The Dell S2716DG and Dell S2716DGR monitors are 27" with a 16:9 aspect ratio. The S2716DG has a resolution of 2560 x 1440 with a 144Hz refresh rate and 1ms response time. Dell's S2716DG is Nvidia G-Sync enabled. The panel used in the Dell S2716DG and S2716DGR is a TN panel with a 350 cd/m^2 lumiance output, 1,000 to 1 contrast ratio supporting 16.7 million colors. Connectivity includes a DisplayPort 1.2 port, HDMI 1.4 port, and built in USB 3.0 hub.
