# Orange Pi 5 Howto
## Download Base Image Ubuntu Jammy for ARM64
download Armbian Jammy	Minimal CLI at https://www.armbian.com/orangepi-5/
## Flash scard and copy image
Write Image via Balena Etcher https://www.balena.io/etcher on sdcard 
## Preparation
Either plug-in a keyboard and a monitor (via hdmi) or do the setup via ssh (usually getting the hostname "orangepi5") or check your router to get the IP
## Login and Create User
default login `moo` password `moothecow`
## Access belaUI via http://[hostname/ip]/
## H265 local SRT
just connect your stream in h265 encoding selecting the proper pipeline using the url `srt:[ip]:1936/publish/live/test`