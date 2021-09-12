# Notes for Installing Package from Blackarch


https://linuxconfig.org/how-to-add-the-blackarch-pentesting-repository-to-arch-linux

## Add the Package Repo

```
# pacman -S curl
$ cd ~/Downloads
$ curl -O https://blackarch.org/strap.sh

$ chmod +x strap.sh

$ sudo ./strap.sh
```

## Install Specific Blackarch Packages
Search
```
$ sudo pacman -Sgg | grep blackarch | cut -d' ' -f2 | sort -u
```

Install
```
$ sudo pacman -S metasploit
```

## Install Entire Categories

Search
```
$ sudo pacman -Sg | grep blackarch
```

Install
```
$ sudo pacman -S blackarch-cryptography
```

