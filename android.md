# Android Mobile Belabox Howto

*Disclaimer this is for Devs because you have to use termux and shell commands*

1. Install Termux from https://play.google.com/store/apps/details?id=com.termux
2. add custom repo and install nginx-rtmp
```
echo "deb [trusted=yes] https://moo-the-cow.github.io/termux-nginx-rtmp/ termux extras" > $PREFIX/etc/apt/sources.list.d/nginx-rtmp.list
apt get update
apt get upgrade
apt install nginx-rtmp
```

Install termux services to activate the nginx on termux startup
```
apt install termux-services openssl-1.1
ln -s $PREFIX/lib/openssl-1.1/libssl.so.1.1 $PREFIX/lib/libssl.so.1.1
ln -s $PREFIX/lib/openssl-1.1/libcrypto.so.1.1 $PREFIX/lib/libcrypto.so.1.1
sv-enable nginx
sv up nginx
```

Install additional belabox packages
```
apt-get install gst-plugins-bad libgstreamer libgstreamer-plugins-base usb-modeswitch nano build-essential git tcl openssl ruby
```

srt
```
git clone https://github.com/BELABOX/srt.git
cd srt
./configure --prefix=$PREFIX
make
make install
cd
```

belacoder
```
git clone https://github.com/moo-the-cow/belacoder.git
cd belacoder
make
cd
```

srtla
```
git clone https://github.com/moo-the-cow/srtla.git
cd srtla
make
cd
```

belaUI
```
git clone https://github.com/moo-the-cow/belaUI.git
cd belaUI
sudo ruby belaUI.rb -o 0.0.0.0 -p 8888
```

Some stuff for the belaUI in ruby
```
gem install sinatra sinatra-contrib thin puma falcon http webrick
```