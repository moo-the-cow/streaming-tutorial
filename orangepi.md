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
### use H265 local SRT via phone (larix/irl pro)
just connect your stream in h265 encoding selecting the proper pipeline in the UI
and in your phone using the url `srt:[ip]:1936/publish/live/test` (publish/live/test being the streamid)
### Setup Wifi on UI
device is autodetected when you plug it it (wlan usb-dongle). you can set it up in the UI. it will only work if you fill all the fields for the device that is detected
