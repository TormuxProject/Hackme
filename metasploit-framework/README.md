## Metasploit Framework Termux
![metasploit](https://camo.githubusercontent.com/da2f4b47699b1c868cf2741fbfbfa5493555cad967793dedbe4f9c78091f2fcc/687474703a2f2f697066732e696f2f697066732f516d594679563353616d3269756959743831796b665a6d684b454c353635714177784e355a4161586b714675424b)

### Installation

> `Wget` ( commandline tool for retrieving files using _HTTP_, _HTTPS_ and _FTP_ )
```
apt install wget
```
> Download from source `Tormux Project`
```
wget https://raw.githubusercontent.com/TormuxProject/Hackme/main/metasploit-framework/metasploit.sh
```
```
chmod +x metasploit.sh
```

### Run
> The script will _configure_ and _setup_ the `metasploit-framework` automatically

```
./metasploit.sh
```

>* If the `download` and `configuration` process is complete
>* `Msf6` is ready to use and don't forget to run [postgresql](../postgresql)

```
msfconsole
```
![metasploit](https://i.ibb.co/JtxG5C8/metasploit.jpg)

> Now you can _generate payload_
```
msfvenom
```
