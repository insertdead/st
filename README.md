# st - simple terminal
st is a simple terminal emulator for X which sucks less.

## Patches
The patches I used are in the patches folder. Some of the patches have 
prerequisites, so make sure to check the page on the suckless 
[website](https://st.suckless.org).

## Requirements
In order to build st you need the Xlib header files. There are also added 
dependencies from the ligatures patch. Go check the ligatures patch page on
[suckless.org](https://st.suckless.org/patches/ligatures/)

## Installation
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):
```
make clean install
```

## Running st
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:
```
tic -sx st.info
```
See the man page for additional details.

## Credits
Based on Aurélien APTEL [aurelien.aptel@gmail.com](mailto:aurelien.aptel@gmail.com) bt source code.
