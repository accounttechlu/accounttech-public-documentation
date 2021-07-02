# AccountTech-Documentation

# How to install Ruby on Rails

## install Ubuntu console in windows


 Open powershell as administrator and run

* dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
* dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

Restart your machine to complete the WSL install

* install Ubuntu from the Microsoft Store

You will then need to create a user account and password for your new Linux distribution.
 
 ## install Ruby

1. sudo apt-get update

2. sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev     software-properties-common libffi-dev

### Install rvm 

1. sudo apt-get install libgdbm-dev libncurses5-dev automake libtool bison libffi-dev
gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB

2. curl -sSL https://get.rvm.io | bash -s stable
source ~/.rvm/scripts/rvm

3.  rvm install 3.0.1

4.  rvm use 3.0.1 --default

5.  ruby -v


* gem install bundler

## Configuring Git

* git config --global color.ui true
* git config --global user.name "YOUR NAME"
* git config --global user.email "YOUR@EMAIL.com"
* ssh-keygen -t rsa -b 4096 -C "YOUR@EMAIL.com"

The next step is to take the newly generated SSH key and add it to your Github account

* cat ~/.ssh/id_rsa.pub

Once you've done this, you can check and see if it worked

* ssh -T git@github.com

## Installing Rails

* curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
* curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

* sudo apt update

* sudo apt-get install -y nodejs yarn

* gem install rails -v 6.1.3.2

* rails -v

## Setting Up PostgreSQL

 Download PostgreSQL for Windows and install it

* sudo apt install libpq-dev

Navigate to the C: drive on Windows. Do this every time you open the Linux console

* cd /mnt/c

* bundle install

## Install nodejs

* sudo apt update

* sudo apt install nodejs

* nodejs -v


## Install Yarn

* sudo apt remove cmdtest

* sudo apt update

* sudo apt install yarn


## Install Redis

* sudo apt update

* sudo apt install redis-server

* sudo nano /etc/redis/redis.conf

find the line specifying the **supervised** directive. By default, this line is set to **no**.
However, to manage Redis as a service, set the supervised directive to **systemd** 

#### restart the Redis service by running

* sudo systemctl restart redis.service

* redis-cli

## PostgreSQL start

* sudo service postgresql start

## Redis Start

* redis-server
