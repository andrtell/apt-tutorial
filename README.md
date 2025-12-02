# apt-tutorial
Ubuntu (Debian) package manager tutorial and cheat-sheet

```
man apt
```
Most of what follows is a summary (or copy) of the various man pages for the `apt` package system.

## User CLI

The `apt` command is designed as an end-user tool. All features of `apt` are available in tools like `apt-get` and `apt-cache` (sometimes more suitable for scripting).

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

