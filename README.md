Useful Commands for Ubuntu
==============

I will list some commands i want to remember here.

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

- Enable or Disable Apache Mods
``` shell
sudo a2enmod module_name
sudo a2dismod module_name
```
