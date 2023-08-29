## Php-Apache

### Installation
```
pkg install php-apache
```
> Create new file in __$PREFIX/etc/apache2/conf.d/__
```
nano $PREFIX/etc/apache2/conf.d/tormux-php.conf
```
>* Copy the following code to that file and save
```
AddHandler php-script .php

ServerName 0.0.0.0

<IfModule dir_module>
        DirectoryIndex index.php
</IfModule>


LoadModule php_module libexec/apache2/libphp.so


<IfModule !mpm_worker_module>
        LoadModule mpm_prefork_module libexec/apache2/mod_mpm_prefork.so
</IfModule>
```
> Press __CTRL + X Y__ enter  to save
```
apachectl start
```
>* PHP-Apache [Error – AH00013 : Pre-configuration failed]
>* Run following command to fix this error
```
sed -i 's|LoadModule mpm_worker|#LoadModule mpm_worker|g' $PREFIX/etc/apache2/httpd.conf
```
> The default Document Root of Apache2 HTTP Server is __$PREFIX/share/apache2/default-site/htdocs__
```
nano $PREFIX/share/apache2/default-site/htdocs/index.php
```
> Write following code and save it
```
<?php
    phpinfo();
?>
```
```
apachectl stop

apachectl start
```

> Delete __index.html__

```
rm $PREFIX/share/apache2/default-site/htdocs/index.html
```
> Open your browser
```
http://localhost:8080/index.php
```
> I'm running on port 8081
 
![php-apache](http://ipfs.io/ipfs/QmPdLKY7tqs3vmkQ7GA5PZMxLnPRswyH1ajMzeJDwirmFt)






