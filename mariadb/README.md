## MariaDB

### Installation
```
pkg install mariadb
```
> Start MySQL Daemon
```
mysqld_safe &
```
```
mysql -u root
```
> Set password on mariadb CLI
```
USE mysql;

set password for 'root'@'localhost' = password('Your_Password');

FLUSH PRIVILEGES;

quit;
```
> Connect from termux CLI and enter your password
```
mysql -u root -p
```

