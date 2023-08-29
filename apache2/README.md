## Apache2 Web Server

### Installation
```
apt install apache2
```

### Run
```
apachectl start
```
![apache2](https://i.ibb.co/ZH9CRvR/apache2.jpg)


### Setup
```
echo "ServerName localhost" >> $PREFIX/etc/apache2
```

> __Stop apache2__
```
apachectl stop
```

> __Run apache2__
```
apachectl start
```

### Port Listening

>* Default `port` is `80`
>* Install `nano text editor`

```
apt install nano
```
```
nano $PREFIX/etc/apache2/httpd.conf
```

> Change the `port 8081`_etc_

![apache-port](https://i.ibb.co/F8JZFKd/apacheport.jpg)

### Save

> CTRL+X Y ENTER


### Web Browser

>* Open your `browser`
>* You can scan it with [nmap](../nmap) if the `port` is `running`

![browser](https://i.ibb.co/T8KVJRc/browser.jpg)

### Apache2 Index Page
```
cd $PREFIX/share/apache2/default-site/htdocs
```
>* Change the index page with basic knowledge of `html` or `php`

>* Runnning `apache2` _http_ to _https_ with [cloudflared](../cloudflared) tunnel
