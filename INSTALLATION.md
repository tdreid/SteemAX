# Instructions for installing SteemAX on Ubuntu 16.04

Be sure to write down the root password that you will create when installing MySQL as you will need it in the following steps. Instructions for setting up the SteemAX database and MySQL user are at the end.

### INSTALL WITH PIP

`sudo apt install python3 python3-pip libssl-dev python3-dev mysql-server`

`pip3 install steemax --user pip`

### INSTALL WITH GIT

`sudo apt install python3 python3-pip libssl-dev python3-dev mysql-server`

`pip3 install steem --user pip`

`git clone https://github.com/ArtoLabs/SteemAX.git`

#### OPTIONAL

`cd ~/SteemAX`

`pip3 install . --user pip`

#### OR RUN AS

`python3 steemax.py`

### SETUP AFTER INSTALL

`mysql_secure_installation`

`mysql -u root -p`

`CREATE DATABASE steemax;`

`CREATE USER 'steemax'@'localhost' IDENTIFIED BY 'SteemAX_pass23';`

`GRANT ALL PRIVILEGES ON steemax.* to 'steemax'@'localhost';`

`exit`



