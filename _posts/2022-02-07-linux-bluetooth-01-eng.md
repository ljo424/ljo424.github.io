---
title: Connect bluetooth device on Linux
subtitle: connect airpods on linux 
date:   2022-02-07 15:40:00 +0800

tag: [linux,note]

thumbnail-img: "/assets/img/markdown-img02.png" #1:1 (450:450)

cover-img: "/assets/img/markdown-turtorial-bg01.png"

#For blog posts, if you want to add a thumbnail that will show up in the feed, use thumbnail-img: /path/to/image. If no thumbnail is provided, then cover-img will be used as the thumbnail. You can use thumbnail-img: "" to disable a thumbnail.
comments: true

# ======= Other parameters ========
layout: post
readtime: true

# test local : bundle exec kyll serve
---
# How to connect airpods on Ubuntu OS

{: .box-note}
**Note:** It's quite eazy , but I forget to push the setup button while connecting to PC LOL ... 

## UI interface 

{: .box-error}
**Error:** Make sure push the setup button on the back of charging case until the status light flash white !

**1. open bluetooth setting on your laptop**

**2. make sure status light flash white while connecting airpods**

**3. connect your airpods!**

## Command line

As an Linux user , using UI interface to connect bluetooth devices is unacceptable (IJK :laughing:

Overall , connecting airpods in command line is coooool !!! :sunglasses:

### bluez

(**BlueZ**)[http://www.bluez.org/]is the official Linux Bluetooth stack. It provides, in it's modular way, support for the core Bluetooth layers and protocols. 

#### install bluez on Ubuntu

```shell
sudo apt install bluez 
```
#### using **bluetoothct** to manage bluetooth devices

run `bluetoothctl` in terminal
```shell
bluetoothctl
```

result :

pic01

Ask what it can do ! Run `help` command

pic02


To connect our headset , we need to first **scan** all the devices nearby , **find** our device ,**pair** the headset and PC, and**connet** it.


{: .box-note}
**Note:** the `[dev]` below means the MAC address of device


* **`exit`**
* **`deivices`**
* **`pair [dev]`**
* **`paired-deivces`**
* **`connect [dev]`**
* **`disconnect [dev]`**



command:
