# XFCE Enviroment at Termux
Give your termux enviroment GUI

![Platform](https://img.shields.io/badge/Platform-Termux-blue?style=flat)
[![Donasi di Trakteer](https://img.shields.io/badge/$-Donate-red?style=flat)](https://trakteer.id/novan245)

## Description
This tutorial helps you to gain access to Linux/Termux applications that require a desktop environment (GUI) to function.
Or to make it easier to use the Termux application so that it is more efficient

## advantages
* Access to GUI applications
* efficient configuration

## Disadvantages
* Not all software can be installed since it's termux
* Minium ram 3GB
<br>

# Installation

<p>First you need to Download and install <a href="https://play.google.com/store/apps/details?id=com.termux">Termux</a> And <a href="https://play.google.com/store/apps/details?id=com.realvnc.viewer.android">VNC Viewer</a> </p>

And then eun this command on termux on by one :
```bash
pkg update pkg upgrade
pkg install x11-repo
```
Install XFCE and VNC Server
```bash
pkg install xfce4 tigervnc
```
Configure VNC server
set the password and port
```bash
vncserver
```
Use nano to modify xstartup to make xfce started on the first run
```bash
nano ~/.vnc/startup
```
then do this
```bash

```



