## PhpMyAdmin
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
