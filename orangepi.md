# Orange Pi 5 Howto
## Download Orange Pi 5 Image
download either an SD image or an USB image see [Streaming Images](https://github.com/moo-the-cow/Streaming-Images)
## Flash scard and copy image
Write Image via Balena Etcher https://www.balena.io/etcher on sdcard 
## Preparation
Either plug-in a keyboard and a monitor (via hdmi) or do the setup via ssh (usually getting the hostname "orangepi5") or check your router to get the IP
## Login and Create User
default login `moo` password `moothecow`

### Access moowss-client UI
enter http://[hostname/ip]/ in your browser
hostname can be orangepi5 or orangepi5plus, but it depends on your router to broadcast those names
+ new Pipelines using SRT (h265 for more quality than RTMP) locallly via phone (larix/irl pro)
just connect your stream in h265 encoding selecting the proper pipeline in the UI
and in your phone using the url `srt:[ip]:1936/publish/live/test` (publish/live/test being the streamid)
+ new Pipelines using HDMI in on orange pi 5 plus
+ new Pipelines for no audio on HDMI in and Camlink
+ Check Wifi Hotspots nearby and list them
+ "Edit Fields" means you can move relevant blocks up and down so you priotize what's on the top yourself. you can always reset that to default.
+ Change Themes
+ Update your System (requires reboot) and get notified when updates are available
+ Setup Wifi on UI
device is autodetected when you plug it it (wlan usb-dongle). you can set it up in the UI. it will only work if you fill all the fields for the device that is detected
+ Export and Import your configuration (for example if you flash your image for backup)

Soon coming:
+ Change the name of your Networking Device (modem) and save it permanently. On Ubuntu 22.04 the devices have unique IDs so this works unlike on the jetson

Screenshots
![grafik](https://github.com/moo-the-cow/streaming-tutorial/assets/34907770/9759133a-ffc3-46d7-b6b3-3dd6c5bbfd52)
![grafik](https://github.com/moo-the-cow/streaming-tutorial/assets/34907770/444a96b0-cc83-4393-aa61-6a3a3d5dd17f)
![grafik](https://github.com/moo-the-cow/streaming-tutorial/assets/34907770/360ec161-774e-40c5-95e0-b702c4d1e4c9)
<img src="https://user-images.githubusercontent.com/34907770/247821232-360ec161-774e-40c5-95e0-b702c4d1e4c9.png" width="60%" />
