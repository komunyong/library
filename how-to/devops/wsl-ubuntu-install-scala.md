# How to add repository in Window Subsystem Linux (Ubuntu:Debien)

## Install packages for add repository command

`apt-get install software-properties-common python-software-properties`

### Repository

1. Install java >= 7

```sh
add-apt-repository ppa:webupd8team/java
apt-get update
apt-get install oracle-java8-installer
```

2. Install scala

```sh
apt-get install scala

wget www.scala-lang.org/files/archive/scala-2.12.3-1.deb
dpkg -i scala-2.12.3-1.deb
apt-get install scala
```

**Reference**: [Install java with CLI](https://stackoverflow.com/questions/32942023/ubuntu-openjdk-8-unable-to-locate-package)
