# Modified to work in recent years

- Temperature & GPU usage monitoring uses HWiNFO Gadget registry (no plugin DLL or paid license needed)
- GPU name detection uses PowerShell (wmic removed from modern Windows)
- Media player uses WebNowPlaying plugin
- Weather uses api.openweathermap.org (add your app id in variables.ini)
- Old readme below

![SysDash Screenshot](http://marcopixel.eu/img/sysDash.png "SysDash Screenshot")

# sysDash
[![GitHub release](https://img.shields.io/github/release/MarcoPixel/sysDash.svg?colorB=97CA00?label=version)](https://github.com/MarcoPixel/sysDash/releases/latest) [![Github All Releases](https://img.shields.io/github/downloads/MarcoPixel/sysDash/total.svg?colorB=97CA00)](https://github.com/MarcoPixel/sysDash/releases) [![GitHub stars](https://img.shields.io/github/stars/MarcoPixel/sysDash.svg?colorB=007EC6)](https://github.com/MarcoPixel/sysDash/stargazers)  [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/MarcoPixel/sysDash/master/LICENSE)

A simple and clean system monitor skin for Rainmeter.


## Minimum Requirements:
- Windows 10 or higher.
- Rainmeter 4.2 (r3018 or higher).
- [HWiNFO](https://www.hwinfo.com/download/) (for CPU/GPU temperatures & GPU usage).


## What's included:
- Clock skin (24hr/12hr)
- CPU & GPU usage
- RAM usage
- Hard drive usage
- Network info (additional variant with just ping and up/download)
- Media player
- Weather skin
- CPU & GPU temperatures
- Recycle bin
- Volume slider

The media player module supports all major media players, including **Spotify** (via WebNowPlaying), **Google Play Music Desktop Player** and **WebNowPlaying** (thanks to @tjhrulz for his plugin) support.

## Important notes

- You need at least **Rainmeter 4.2 (r3018) or higher** to get all features of this skin. You can find the newest version on https://www.rainmeter.net/
- After installation you can access the settings by right-clicking on one of the skins then clicking on Open Settings.
- If there are no skins loaded, you have to reinstall the skin and check if the layout is getting loaded after install.

## Temperature & GPU usage setup (HWiNFO)

The CPU/GPU temperature and GPU usage skins require **[HWiNFO](https://www.hwinfo.com/download/)** (free for personal use) running in the background. The skin reads sensor data from HWiNFO's **Gadget** registry reporting — no extra plugin DLLs or paid licenses needed.

### Quick setup

&nbsp;&nbsp;&nbsp;**1.** Install and launch [HWiNFO](https://www.hwinfo.com/download/) in **Sensors-only** mode.

&nbsp;&nbsp;&nbsp;**2.** In the sensors window, click the **gear icon** (Settings) at the bottom.

&nbsp;&nbsp;&nbsp;**3.** Go to the **HWiNFO Gadget** tab.

&nbsp;&nbsp;&nbsp;**4.** For each sensor you want, **tick the checkbox** to enable reporting. At minimum enable:
- Your **CPU Package** (or CPU Tctl/Tdie) temperature
- Your **GPU Temperature**
- Your **GPU Utilization** (for the GPU usage graph)

&nbsp;&nbsp;&nbsp;**5.** Note the **index number** assigned to each (starting from 0).

&nbsp;&nbsp;&nbsp;**6.** In SysDash, right-click any skin > **Open Settings** > **HWiNFO** tab, and enter those index numbers.

&nbsp;&nbsp;&nbsp;**7.** Set HWiNFO to start with Windows (Settings > General > Auto Start).

For a detailed walkthrough, see the [official Rainmeter HWiNFO guide](https://docs.rainmeter.net/tips/hwinfo/).

## Getting started

### Automatic installation

&nbsp;&nbsp;&nbsp;**1.**  Download the latest skin here: https://github.com/MarcoPixel/SysDash/releases

&nbsp;&nbsp;&nbsp;**2.**  Install the skin by **double-clicking** the .rmskin file and going through the installer.

&nbsp;&nbsp;&nbsp;**3.**  After finishing the setup Rainmeter will load the basic layout and the settings skin where you can access additional options.

&nbsp;&nbsp;&nbsp;**4.**  You're done! Enjoy your new Rainmeter skin!

### Manual installation

&nbsp;&nbsp;&nbsp;**1.**  Clone this repo to **Documents\Rainmeter\Skins**.

&nbsp;&nbsp;&nbsp;**2.**  Go to **.installer\plugins** and then move the 32 or 64-bit plugins (depending on your system) to &nbsp;&nbsp;&nbsp;**AppData\Roaming\Rainmeter\Plugins**.

&nbsp;&nbsp;&nbsp;**3.**  Launch Rainmeter and right-click the tray icon, press Themes and open the **SysDash** theme.

&nbsp;&nbsp;&nbsp;**4.**  You're done! Enjoy your new Rainmeter skin!

## Issues & feature requests

If you still have issues or a bug, please report them [here](https://github.com/MarcoPixel/SysDash/issues). Be sure to include details like the operating system, Rainmeter version and logs so we can help you as much as we can.

You can also request new features and help them develop by joining the discussion. Just add the **request label** to your issue and we will have a look!

#### [Click here to get to the open issues](https://github.com/MarcoPixel/SysDash/issues).

### Credits
- **Rainmeter Skin** - **[@marcopixel]**(https://github.com/marcopixel) 
- **HWiNFO Plugin** - stangowner (https://www.hwinfo.com/forum/Thread-Rainmeter-plug-in-for-HWiNFO-3-2)
- **Google Play Music Desktop Player Plugin** - **[@tjhrulz](https://github.com/tjhrulz/GPMDP-Plugin)**
- **WebNowPlaying Plugin** - **[@tjhrulz](https://github.com/tjhrulz/WebNowPlaying)**
- **Fonts** - Uni Sans & Uni Neue from fontfabric.com
- **Icons** - Feather icons (https://github.com/colebemis/feather) & [Jelle-Dekkers](http://jelle-dekkers.deviantart.com/) (GPU icon)
- **Weather Icons** - Climacons (http://adamwhitcroft.com/climacons/)
- **Wallpaper** - [Mariusz Potocki](http://potocki.com.pl/outdoor/)
- Thanks to **@khanhas** for providing his graph code and @undefinist for the refresher code.
