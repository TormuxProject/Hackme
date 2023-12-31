## PhpMyAdmin
![phpmyadmin](https://i0.wp.com/saixiii.com/wp-content/uploads/2017/04/logo-phpmyadmin.png?ssl=1)

### Installation
```
pkg install php phpmyadmin mariadb
```
> The path for PhpMyAdmin is
```
$PREFIX/share/phpmyadmin
```
> Or
```
/data/data/com.termux/files/usr/share/phpmyadmin/
```
### Configuration
```
cd $PREFIX/share/phpmyadmin
```
```
nano config.inc.php
```
>* Find the configuration host and add port 3306 after localhost

![phpmyadmin](http://ipfs.io/ipfs/QmVUgqHgQHAitXgkPuXoknDfLhU1GK4aKFgz6uKDNJipkt)

> Start MariaDB Server in background
 ```
mysqld_safe &
```
> Start PHP Server in PHPMyAdmin directory
```
php -S localhost:8080 -t $PREFIX/share/phpmyadmin/
```
> Open browser localhost:8080

![phpmyadmin-browser](https://ipfs.io/ipfs/QmXU2zbfsG8gpuPvafJ4f3Jr5qhybLgDXHE8YoSTSLYAdL)
