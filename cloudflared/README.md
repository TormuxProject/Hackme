## Cloudflared Termux
![cloudflared](https://logos-marques.com/wp-content/uploads/2021/03/Cloudflare-Logo.png)

### Installation
```
apt install cloudflared
```

> Install `apache2` web server
```
apt install apache2
```

### Run

> [Apache2](../apache2) web server
``` 
apachectl start
```

> CLoudflared tunnel
```
cloudflared tunnel --url localhost:8080
```

>* Your quick `Tunnel` has been `created`! Visit it at (it may take some time to be reachable):

>* Copy `trycloudflare.com` url link and paste it in your browser

![cf](https://i.ibb.co/D93Kcmm/cloudflared.jpg)

## Stop

> __Cloudflared__
```
CTRL + C
```

> __Apache2 server__
```
apachectl stop
```
