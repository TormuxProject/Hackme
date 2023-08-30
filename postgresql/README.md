## Postgresql Termux
![postgresql](https://www.myintervals.com/blog/wp-content/uploads/2011/12/postgresql-logo1.png)

### Installation

```
apt install postgresql
```

### Skeleton Database

```
mkdir -p $PREFIX/var/lib/postgresql
```
```
initdb $PREFIX/var/lib/postgresql
```

### Run

> `Starting` the `database`
```
pg_ctl -D $PREFIX/var/lib/postgresql start
```

> `Stopping` the `database`
```
pg_ctl -D $PREFIX/var/lib/postgresql stop
```
>* `Postgresql` can be run with [metasploit-framework](../metasploit-framework)

>* You can scan it with [nmap](../nmap) if the `port` is `running`
