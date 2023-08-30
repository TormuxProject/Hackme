## Kali Linux Gui Desktop
![kali](https://www.unixmen.com/wp-content/uploads/2015/11/Kali_Linux_Logo.png)

### Installation

> Before running `kali linux gui desktop` you have to install [nethunter-rootless](../nethunter-rootless) and download [vnc-viewer](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android)  

```
nh
```
```
sudo apt install udisks2 xfce4 xfce4-whiskermenu-plugin qterminal dbus-x11 firefox-esr tigervnc-standalone-server kali-themes tightvncserver xfce4*
```

> Remove `udisks2.postinst` and echo with blank text
```
sudo rm /var/lib/dpkg/info/udisks2.postinst
```
```
echo "" >> /var/lib/dpkg/info/udisks2.postinst
```

> Configure ( _dpkg_ )
```
sudo dpkg --configure -a
```
```
apt-mark hold udisks2
```

> Remove _xstartup_ file and _adding bash script_ ( save it __CTRL+X Y ENTER__ )
```
rm .vnc/xstartup
```
```
nano .vnc/xstartup
```

```
#!/bin/bash
startxfce4 &
```

![xstartup](https://i.ibb.co/8Y2RMD7/xstartup.jpg)

### Vncstart

> Make a command in `/usr/bin/` to make it easier to run _vncserver_ ( save it __CTRL+X Y ENTER__ )

```
sudo nano /usr/bin/vncstart
```

```
vncserver -geometry 1920x920 -xstartup /usr/bin/xfce4-session :1
```

![vncstart](https://i.ibb.co/xjWv5j4/vncstart.jpg)

```
sudo chmod +x /usr/bin/vncstart
```

### Vncstop

```
sudo nano /usr/bin/vncstop
```

```
vncserver -geometry 1920x920 -xstartup /usr/bin/xfce4-session -kill :1
```

![vncstop](https://i.ibb.co/k2ZRYK6/vncstop.jpg)

```
sudo chmod +x /usr/bin/vncstop
```

### Run

> Start `vncserver`

```
vncstart
```

> Stop `vncserver`

```
vncstop
```

![vncstart](https://i.ibb.co/7XV7P60/vncstart.jpg)

### Vnc viewer

> Set `localhost:1` and name ( _anything_ )

![localhost](https://i.ibb.co/MMycL11/lhost.jpg)

> Picture quality ( _high_ )

![HQ](https://i.ibb.co/FVjX5JF/hq.jpg)

> `Vncstart` ( _password_ ) and _continue_

![pwd](https://i.ibb.co/5kW182p/pwd.jpg)

### `Kali linux Desktop`

![kalilinuxguidesktop](https://i.ibb.co/61K0Lck/kali-linux-gui-desktop.jpg)
