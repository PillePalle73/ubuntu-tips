just some hints for troubleshooting ubuntu

Listen neu:
sudo rm -rf /var/lib/apt/lists/*
sudo apt-get update

Runterladen,nicht installieren:
sudo apt-get dist-upgrade -d


Brother DCP-357CW:
https://forums.linuxmint.com/viewtopic.php?t=46302

https://forum.ubuntuusers.de/topic/brother-dcp-375cw-scanner-wird-trotz-treiberin/

https://wiki.ubuntuusers.de/Scanner/Brother/


64bit-Treiber im falschen Ordner, also:

sudo ln -sf /usr/lib64/sane/libsane-brother* /usr/lib/x86_64-linux-gnu/sane
sudo ln -sf /usr/lib64/libbrcolm* /usr/lib/x86_64-linux-gnu
sudo ln -sf /usr/lib64/libbrscandec* /usr/lib/x86_64-linux-gnu

brscan-skey -l 
