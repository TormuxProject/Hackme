## Termux Properties

### Installation

> `Wget` ( commandline tool for retrieving files using _HTTP_, _HTTPS_ and _FTP_ )
```
apt install wget
```

### Setup

> If the `termux.properties` file is not found then go to the next step

```
rm .termux/termux.properties
```

> If the `.termux` folder doesn't exist then create the folder first

```
mkdir .termux
```

> Retrieving ``termux.properties`` file to folder `.termux`
```
wget https://raw.githubusercontent.com/TormuxProject/Hackme/main/termux.properties/config/termux.properties -P .termux
```

### Reload Settings
```
termux-reload-settings
```

### Handling Terminal Sessions

__CTRL+T__ Create session

__CTRL+N__ Rename session

__CTRL+1__ Previous session

__CRTL+2__ Next session

### Handling Extra Keys

__CTRL+A__  Move cursor to the beginning of line

__CTRL+C__  Abort (send SIGINT to) current process

__CTRL+D__  Logout of a terminal session

__CTRL+E__  Move cursor to the end of line

__CTRL+K__  Delete from cursor to the end of line

__CTRL+U__  Delete from cursor to the beginning of line

__CTRL+L__  Clear the terminal

__CTRL+Z__  Suspend (send SIGTSTP to) current process

__CTRL+W__  Clear prompt before word (a word is a set of characters after a space)
