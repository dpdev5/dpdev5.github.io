---
layout: single
title: Delivery - Hack The Box
excerpt: "Delivery is a quick and fun easy box where we have to create a MatterMost account and validate it by using automatic email accounts created by the OsTicket application. The admins on this platform have very poor security practices and put plaintext credentials in MatterMost. Once we get the initial shell with the creds from MatterMost we'll poke around MySQL and get a root password bcrypt hash. Using a hint left in the MatterMost channel about the password being a variation of PleaseSubscribe!, we'll use hashcat combined with rules to crack the password then get the root shell."
date: 2021-09-01
classes: wide
header:
  teaser: /assets/images/htb-writeup-delivery/delivery_logo.png
  teaser_home_page: true
  icon: /assets/images/hackthebox.webp
categories:
  - ROMS
  - TWRP
  - MIUI 12.5
tags:  
  - onclite
  - redmi
  - xiaomi
  - xiaomi redmi 7
  - twrp
  - MIUI 12.5
---

![](/assets/images/htb-writeup-delivery/delivery_logo.png)

# Presenting onclite MIUI12 updater




## Disclamer

```
I am not responsible for bricked devices, dead SD cards,
thermonuclear war, or the current economic crisis caused by you following
these directions. YOU are choosing to make these modificiations, and if
you point your finger at me for messing up your device, I will LMAO at you.
```

### Objective

The purpose of this tool is to install the much desired MIUI12 on Xiaomi Redmi 7 (onclite) devices.

### Python dependencies
To use this tool you must have Python installed, if you don't have it, you can download it from the official website:
https://www.python.org/downloads/

You will also need to install the necessary dependencies, in this case they are:

 - tqdm




To install tqdm, open a terminal or cmd and type the following command:

    pip install tqdm

> If there is any other problem with another dependency we will use the
> same command but changing the name of the dependency.

### Adb and fastboot
To use the tool you must have the adb and fastboot drivers installed. 
#### Windows
https://forum.xda-developers.com/t/official-tool-windows-adb-fastboot-and-drivers-15-seconds-adb-installer-v1-4-3.2588979/

#### Ubuntu



## Getting started in Windows
First we download the folder with the code in zip format or we make a clone using git

If we have downloaded the zip, we extract it and enter the resulting folder, if we have done a clone we don't have to extract anything.

Now we connect the phone in Fastboot mode (press the volume down and power button at the same time until it appears on the Fastboot screen).

![Fastboot Xiaomi](https://tuxiaomi.es/wp-content/uploads/2021/03/Fastboot-Xiaomi-1.jpg)

Now we run the app.py file and follow the steps





## Getting started in Linux / Mac OS

First we download the folder with the code in zip format or we make a clone using git

If we have downloaded the zip, we extract it and enter the resulting folder, if we have done a clone we don't have to extract anything.

Now we connect the phone in Fastboot mode (press the volume down and power button at the same time until it appears on the Fastboot screen).

![Fastboot Xiaomi](https://tuxiaomi.es/wp-content/uploads/2021/03/Fastboot-Xiaomi-1.jpg)

Now open a terminal in the folder containing the app.py file and type the following command


    python3 app.py
    

## Video-guide installing MIUI 12.5 
https://youtu.be/LtCEpc4mPiQ

## Other versions
You can download other versions on releases section
