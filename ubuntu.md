# all Ubuntu OS packages installed on the server are up to date

> apt-get update
> apt-get upgrade

## install OpenJDK

> apt install openjdk-17-jdk openjdk-17-jre
> java -version

## find java home

> sudo find / -type f -name java

## git clone with branch 

> git clone --depth 1 --branch 392 https://github.com/trinodb/trino.git

## list file/folder size in order

> ls -lrha | more
