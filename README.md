Useful Commands for Ubuntu
==============
I will list some commands i want to remember here. Please contribute related commands, if you like.

Media Functions
--------------
- Install ubuntu-restricted-extras (for mp3, unrar, flash etc together)
``` shell
sudo apt-get install ubuntu-restricted-extras
```

- Install mp3 support
``` shell
sudo apt-get install libmp3lame0
```

- Install Flashplugin
``` shell
sudo apt-get install flashplugin-installer
```

- Install DVD Codecs (Note: libdvdread4 may be installed with ubuntu-restricted-extras already)
``` shell
sudo apt-get install libdvdread4
sudo /usr/share/doc/libdvdread4/install-css.sh
```
reboot then

Managing Packages
--------------

- Search the installed packages
``` shell
dpkg-query -l *searchstring*
```

- Search the Packages to install
``` shell
apt-cache search searchstring
```

Useful Packages
-------------
- Install to open terminal from file manager in right-Click context menu.
``` shell
sudo apt-get install nautilus-open-terminal 
```

Managing Webserver
--------------
- Search included Php extensions
``` shell
grep -Hrv ";" /etc/php5 | grep -i "extension="
```

- Enable or Disable Php extensions
``` shell
sudo php5enmod ext_name
sudo php5dismod ext_name
```

- Search included Apache2 modules
``` shell
apache2ctl -M
```

- Enable or Disable Apache Mods
``` shell
sudo a2enmod module_name
sudo a2dismod module_name
```
Finding Hardware
----------------

- Motherboard
``` shell
sudo dmidecode -t 2
```

Error handling
---------
Restart Pulseaudio
``` shell
pulseaudio -k
pulseaudio --start
```
