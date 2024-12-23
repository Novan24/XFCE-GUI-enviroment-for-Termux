# XFCE Enviroment at Termux
Give your termux enviroment GUI

[![contact](https://img.shields.io/badge/contact-green?style=flat)](085735101561)

![Platform](https://img.shields.io/badge/Platform-Termux-blue?style=flat)
[![Donasi di Trakteer](https://img.shields.io/badge/$-Donate-red?style=flat)](https://trakteer.id/novan245)

## Description
This tutorial helps you to gain access to Linux/Termux applications that require a desktop environment (GUI) to function.
Or to make it easier to use the Termux application so that it is more efficient

## Who is it for?
* to run spesific, but compatible apps that require GUI enviroments
* maybe you come here to run inkscape on mobile device

## Note
* Not all software can be installed since it's termux
* Performance and compatibilty really depends on device or termux version is used
<br>

# Installation

<p>First you need to Download and install <a href="https://play.google.com/store/apps/details?id=com.termux">Termux</a> And <a href="https://play.google.com/store/apps/details?id=com.realvnc.viewer.android">VNC Viewer</a> </p>

And then copy, paste this command on termux one by one, also while following the instruction on screen, usually type "Y" then Enter, while upgrading or installing  :
<br>
1. to update and upgrade package repository
   and access to x11-repo
```bash
pkg update && pkg upgrade
pkg install x11-repo
```

2. Install XFCE and VNC Server
```bash
pkg install xfce4 tigervnc
```
3. Configure VNC server
set the 6 digits password,
don't worry, the password is typed even if you can't see it
```bash
vncserver
```
[![vncserver.jpg](https://i.postimg.cc/59XrPcvs/IMG-20241223-102553.jpg)](https://postimg.cc/Yjw89sdF)

4. Use nano to modify xstartup to make xfce started on the first run
```bash
nano ~/.vnc/xstartup
```
5. then copy, paste like in the image below:
```bash
xrdb $HOME/.Xresources
startxfce4 &
```
[![Example.png](https://i.postimg.cc/2jgKMH7r/IMG-20241223-102655.jpg)](https://postimg.cc/Hj4z79Nh)
then CTRL+X > Y > Enter
<br>
6. Start your vncserver, default is 1
```bash
vncserver :1
```

7. Open RVNC server app > click + > Enter this Address: localhost:5901, Name > Create > Enter password > and you will come out with this :
[![IMG-20241222-213824.jpg](https://i.postimg.cc/h4pf44ns/IMG-20241222-213824.jpg)](https://postimg.cc/kDRnfmBR)

8. and don't forget to turn off the server after using it
```bash
vncserver -kill :1
```

## #FAQ 
1. There is error while doing `pkg update && pkg upgrade`
 ```
 Make sure to download termux version
 that working on your device,
 you can find it on the internet
 ```
2. the screen shows black when the first time i run the VNC
```
Make sure you type the bash code
in the right place like i shown
in the image on step 5.
```

3. download inkscape after all the tutorial were done.
   ```
   pkg install inkscape
   ```

## End.
that's it to help you be able to give your termux GUI 🎉

<br>

If you have any issues please <a href="">Contact me</a> via whatsapp or
<br>
My email : graphdesigner25@gmail.com

<br>

[![Donasi di Trakteer](https://img.shields.io/badge/Buy_me_a-Cendol-red?style=for-the-badge)](https://trakteer.id/novan245)
