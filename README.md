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

And then use this command on termux one by one :
<br>
1. 
```bash
pkg update pkg upgrade
pkg install x11-repo
```

2. Install XFCE and VNC Server
```bash
pkg install xfce4 tigervnc
```
3. Configure VNC server
set the password and port
(You need to remember password and port that you configure for Rvnc app)
```bash
vncserver
```
4. Use nano to modify xstartup to make xfce started on the first run
```bash
nano ~/.vnc/startup
```
5. then copy and paste like this
```bash
xrdb $HOME/.Xrecources
startxfce4 &
```
[![Example](https://i.postimg.cc/BnK1YWF0/IMG-20241222-194444.jpg)](https://postimg.cc/nXnzrPTR)
then CTRL+X > Y > Enter
<br>
6. Start vncserver
```bash
vncserver :1
```
and don't forget to turn off the server just like you turn off your pc
```bash
vncserver -kill :1
```
