---
layout: page
title: Evil Portals
tagline: 
description:
---

## Evil Portals

A collection of portals that can be loaded into the Evil Portal module and can be used to capture credentials Wifi using the [Hak5](https://hak5.org/) [Wifi Pineapple](https://wifipineapple.com/) [Tetra](http://hakshop.myshopify.com/products/wifi-pineapple?variant=11303845317) and [Nano](http://hakshop.myshopify.com/products/wifi-pineapple?variant=81044992).

This project requires you to manually install the development branch of the [Evil Portal](https://github.com/frozenjava/EvilPortalNano/tree/development) captive portal module created by [frozenjava](https://github.com/frozenjava).

### Usage

Clone the repository

`git clone https://github.com/kbeflo/evilportals`

Change directory to evilportals/portals/

`cd evilportals/portals/`

Copy the portals you wish to use on the Tetra at `/root/portals/` or on the Nano at `/sd/portals/`

    scp -r portal-login root@172.16.42.1:/root/portals/

Alternatively you can use [Filezilla](https://filezilla-project.org/) to copy the portals

Host: `sftp://172.16.42.1` Username: `root` Password: `lamepassword` Port: `22`  

After gathering credentials, captured data will be stored on the Tetra at `/root/evilportal-logs/portal-login.txt` or on the Nano at `/sd/evilportal-logs/portal-login.txt`

---

