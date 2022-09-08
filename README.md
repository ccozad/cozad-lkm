# cozad-lkm
 Linux kernel module programming for busy people
 
# Introduction 
This repo is dedicated to short tutorials about Linux kernel module development. We'll focus on getting up and running fast. After you have learned the basics there are links you can read to gain a deeper understanding.

# Setup
You are going to need a Linux install that you are ok breaking. There are at least 20 different ways to go about solving this problem, two paths are presented for simplicity.

1. If you have a nice computer (maybe a good gaming rig), install Virtual Box and run Ubuntu on a virtual machine
2. If you don't have a nice computer, get a cheap computer and install Ubuntu on it

## Install Ubuntu on a virtual machine

Follow these instructions on [How to run Ubuntu on a virtual machine](https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox#1-overview)

## Install Ubuntu on physical hardware 

Follow the instructions on [How to install Ubuntu Desktop](https://ubuntu.com/tutorials/install-ubuntu-desktop#1-overview)

## Install tools

 - For simplified editing we'll use Visual Studio code for all of our exercises. The Ubuntu Store should have a Visual Studio available as a one click install
 - Ubuntu has a program called "Terminal". Click the icon in the left corner to access installed applications. Commands are listed in this type of formatting `<type this command into the terminal`
 - You need tools to compile kernel modules `sudo apt-get install build-essential kmod`
 - You will also need headers for your kernel `sudo apt-get update` then `apt-cache search linux-headers-`uname -r``
 - You will also need git to retrieve the samples and version your work `sudo apt install git`
 
# Organization
The tutorials are easiest to understand if you follow the recommended order. If that is too slow there is a cheat sheet with key ideas that can help you skip lessons.

1. [Hello World v1](/hello-1) Simplest Kernel module you can make
2. [Hello World v2](/hello-2) Custom entry and exit definitions

# FAQ

## How can I get more detail?
This content is a simplified form of notes from the [Linux Kernel Programming Guide](https://sysprog21.github.io/lkmpg/)

## Why aren't you using Linux distro X?
The are tons of great distros out there. Maybe you are a purist that likes a clearn arch distro or you like Fedora over Ubuntu. These tutorials are designed to get beginers up and running fast. Learners can delve into the evolving world of Linux distros later.

## Why are you suggesting to use Visual Studio Code as an IDE and not a terminal editor?
I remember my first time learning low level Linux development. The instructor spent multiple class periods explaining the intricacies (and quirks) of using vi when really I wished we had spent more time talking about the foundation concepts of OS internals.

## I found an error, what do I do?
File a bug or submit a pull request
