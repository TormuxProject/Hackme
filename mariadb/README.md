## MariaDB
![mariadb](https://meterpreter.org/wp-content/uploads/2018/08/mariadb.png)

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
> Set Flush Privileges root on mariadb CLI for set your password
```
USE mysql;

set password for 'root'@'localhost' = password('Your_Password');

flush privileges;

quit;
```
> Connect from termux CLI and enter your password
```
mysql -u root -p
```
> You can running [phpmyadmin](../phpmyadmin) after install mariadb and phpmyadmin with your root and password to access GUI phpmyadmin

