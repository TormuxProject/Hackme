## Metasploit Framework Termux

### Installation

> `Wget` ( commandline tool for retrieving files using _HTTP_, _HTTPS_ and _FTP_ )
```
apt install wget
```
> Download from source `Tormux Project`
```
wget https://raw.githubusercontent.com/tormux-project/tormux-project/main/metasploit-framework/metasploit.sh
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
