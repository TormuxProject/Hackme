## OpenSSH

### Installation
```
apt install openssh
```
> Before running `ssh` first create a `passwd` to _login_

![passwd](https://i.ibb.co/fVWw9ch/passwd.jpg)

### Run
```
sshd
```

>* Use [nmap](../nmap) to see if `ssh` is _running_

>* `ssh` on _termux_ running on port `8022`

>* For the _username_ ( anything )

>* Connect with other _devices_

>* The tools used as in the picture are [nethunter-rootless](../nethunter-rootless) and [tmux](../tmux)

```
ssh -p 8022 tormuxproject@localhost
```

![openssh](https://i.ibb.co/Kyvj5Cp/openssh.jpg)

> Stopping `ssh`
```
pkill sshd
```

### More Information
> [Openssh](https://wiki.termux.com/wiki/Remote_Access) on wiki termux
