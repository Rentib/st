## st - simple terminal
st is a simple terminal emulator for X which sucks less.

## Patches
This build of st comes with the following patches:
* [alpha](./patches/st-alpha-20220206-0.8.5.diff)
* [appsync](./patches/st-appsync-20200618-b27a383.diff)
* [boxdraw](./patches/st-boxdraw_v2-0.8.5.diff)
* [desktopentry](./patches/st-desktopentry-0.8.5.diff)
* [expected anysize](./patches/st-expected-anysize-0.9.diff)
* [ligatures](./patches/st-ligatures-alpha-scrollback-ringbuffer-20230105-0.9.diff)
* [scrollback ringbuffer](./patches/st-scrollback-ringbuffer-0.8.5.diff)
* [netwmicon](./patches/st-netwmicon-0.8.5-v2.diff)
* [newterm](./patches/st-newterm-0.9.diff)
* [xresources signal reload](./patches/st-xresources-signal-reloading-20220407-ef05519.diff)

## Requirements
In order to build st you need the Xlib header files.

## Installation
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install

## Running st
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

## Credits
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
