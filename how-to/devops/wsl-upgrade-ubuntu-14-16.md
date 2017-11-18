# How to upgrade Window Sub System from Ubuntu 14.04 to 16.04

## Required

1. Window v.1703 (OS Build 15063.xxx+)
2. Backup all config file in your old WSL.

## Process

1. open powershell
2. `lxrun /uninstall /full`
3. `lxrun /install`

**Note**:

Check Ubunbu running version `lsb_release -a`

Check window version by push 
  - [Window] button
  - typing `winver`
  - [Enter]

**References**: https://blogs.msdn.microsoft.com/commandline/2016/10/19/wsl-adds-ubuntu-16-04-xenial-support/
