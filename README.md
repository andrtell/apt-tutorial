# APT Tutorial
Ubuntu (Debian) package manager tutorial and cheat-sheet

```
man apt
```
Most of what follows is a summary (or copy) of the various man pages for the `apt` package system.

## User CLI

The `apt` command is designed as an end-user tool. 

All features of `apt` are available in tools like `apt-get` and `apt-cache` (offers more control).

### System
These commands work on the system as a whole.
```
apt update
```
Download package information from all configured sources.
```
apt upgrade
```
Install available upgrades of all packages installed.
```
apt full-upgrade
```
Install upgrades and also remove installed packages if needed to upgrade system.
```
apt autoremove
```
Remove packages that are no longer needed.

### Sources
To install a package from a source that is maintained by a third-party, your first need to add that source.
```
man add-apt-repository
```
Sources can be added or removed by using the `add-apt-repository` command.
```
add-apt-repository -P neovim-ppa/stable
```
Add a new PPA source.
```
apt update
apt install neovim
```
Do not forget to run `apt update` after adding a source.
```
add-apt-repository -P -r neovim-ppa/stable
```
Remove a PPA source.

```
add-apt-repository -L | less
```
List APT sources.
```
ls /etc/apt/sources.list.d/*
```
See `man sources.list` for working with source-files directly.