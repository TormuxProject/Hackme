## Nmap
![nmap](https://camo.githubusercontent.com/1f24f723d642f3ae37a9676ed7d130998c1d6f8f1b8bbc383ce45515d8705521/68747470733a2f2f697066732e696f2f697066732f516d64566247667239695556323878485932546338337842556155716d44764877596f3344334e4435533667616f)

### Installation
```
apt install nmap
```

### Run
```
nmap testphp.vulnweb.com
```

![nmap](https://i.ibb.co/5B8XGYJ/nmap.jpg)

>* Port `80` open

>* Try with `-A` _Enable OS detection_, _version detection_, _script scanning_, and _traceroute_

>* `-p` Only scan specified ports

```
nmap testphp.vulnweb.com -p80 -A
```

![nmap](https://i.ibb.co/dGfKLSr/nmap.jpg)

> Can be used to `scan` your `network` ( _localhost_ ), such as [postgresql](../postgresql), [apache2](../apache2), and [ssh](../openssh) etc

```
nmap localhost
```

### More Information

> [Nmap](https://nmap.org/book/man.html) the network mapper
