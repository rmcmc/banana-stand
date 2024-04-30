# Raspbery Pi Setup

## What Pi

I've got a pi 5 with 8GB RAM. Running on a 8gb micro SD (to be expanded)

## Loading distro
I'm using raspberry pi imager to set up an Ubuntu LTS Server 24.04. Pre populating the wifi credential, UID and SSH. This seems easier than trying to set up via command line which seemed to cause issues with wifi.

I've chosen the server version of Ubuntu over other options as this appears more widely applicable to the wider world beyond the pi.

## First boot

Run `sudo apt update`

### Set Up SSH

`sudo apt install openssh-server`

`sudo ufw allow ssh`

`hostname -I`

Then on laptop

`ssh uid@ip.from.hostname`

## Postgresql Setup

I've decided to host all DBs on postgres https://ubuntu.com/server/docs/install-and-configure-postgresql

`sudo apt install postgresql`
