## Nmap

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
