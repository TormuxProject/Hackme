## Php-Apache

### Installation
```
pkg install php-apache
```
> Create new file in __$PREFIX/etc/apache2/conf.d/__
```
nano $PREFIX/etc/apache2/conf.d/tormux-php.conf
```
>* Copy the following code to that file and save.
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
