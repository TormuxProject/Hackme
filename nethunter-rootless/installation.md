## Nethunter Rootless

### Installation
```
termux-setup-storage
```
> `Termux-setup-storage` in order to have access to shared storage

```
apt install wget
```
```
wget https://raw.githubusercontent.com/tormux-project/tormux-project/main/nethunter-rootless/config/nethunter
```

> `Wget` ( commandline tool for retrieving files using _HTTP_, _HTTPS_ and _FTP_ )

```
chmod +x nethunter
```

> Give the file _permission_ to be _executed_

### Run

```
./nethunter
```

![nethunter](https://i.ibb.co/zZMLHTj/nethunter.jpg)

> Follow the steps and until the download is complete

### Usage

Open termux and type one of the following command

* `nethunter -r` start Kali NetHunter cli as root

* `nh -r` start Kali NetHunter cli as root

* `nethunter` start Kali NetHunter command line interface ( nonroot )

* `nh` start Kali NetHunter command line interface ( nonroot )

* `nethunter kex passwd` configure the KeX password (only needed before 1st use)

* `nethunter kex &` start Kali NetHunter Desktop Experience user sessions

* `nethunter kex stop` stop Kali NetHunter Desktop Experience

### More Information

> You can run [nethunter gui desktop](../nethunter-gui-desktop) or [kali linux gui desktop](../kali-linux-gui-desktop) after installing _nethunter rootless_

![kali](https://i.ibb.co/MswyhmR/kali.jpg)
