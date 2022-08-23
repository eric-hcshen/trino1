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

> du -sh *

## split large file to small files

> split -b 10M trino.tar "trino.tar.part"
> 
> cat trino.tar.part* > trino.tar.joined

## Github ssh
[SSH to Github](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

> ssh-keygen -t ed25519 -C "eric.hcshen@gmail.com"
> 
> eval "$(ssh-agent -s)"
> 
> ssh-add ~/.ssh/id_ed25519
> 
> cat ~/.ssh/id_ed25519.pub
> 
> git remote add origin git@github.com:eric-hcshen/trino1.git
