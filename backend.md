## Starting and Stopping psql service
sudo systemctl start postgresql.service
sudo systemctl status postgresql.service
sudo systemctl restart postgresql.service
systemctl stop postgresql

sudo pg_isready //to know the server port

## installing jdk11
refer:
https://www.linuxshelltips.com/set-java_home-path-ubuntu/
https://www.linode.com/docs/guides/how-to-install-openjdk-on-ubuntu-20-04/
set path variable
setting select jdk11 in intelliJ

## Starting psql shell in terminal

Switch over to the postgres account on your server by typing:

> sudo -i -u postgres psql
You can now access the PostgreSQL prompt immediately by typing:

> psql

### Change password of the user
> \password
From there you are free to interact with the database management system as necessary.

Exit out of the PostgreSQL prompt by typing:
>postgres=# \q

## Installing maven on linux

wget https://mirrors.estointernet.in/apache/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.tar.gz
tar -xvf apache-maven-3.6.3-bin.tar.gz
mv apache-maven-3.6.3 /opt/

ref: https://www.digitalocean.com/community/tutorials/install-maven-linux-ubuntu

## kill a prot
 sudo kill -9 `sudo lsof -t -i:5432`

## Minimal ExpressJs Setup

 > touch entryPoint.js
 > npm init
 > npm i express

 Add following snippet:
 "
 const express = require('express')
 const app = express()
 const port = 3000
 "

 > nodemon fileName.js //install nodemon if not exist
