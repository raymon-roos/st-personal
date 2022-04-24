# Welcome to my personal build of st

This project exists to house my personal patched version of [st][1] and make it easily
accessible for all my devices in the future and gain familiarity with github. Original
[readme][2] included below.

[1]: https://st.suckless.org/ "st homepage"
[2]: https://git.suckless.org/st/ "st sourcecode"

### Patches applied are (in no particular order)
> - [st-delkey][3] Make the delete and backspace keys do what you expect
> - [st-anysize][4] Prevent unseemly edges along terminal inner border as the window
>   changes shape/size
> - [scrollback][5] Allow scrolling back through the console history
> - [gruvbox][6] Cool retro colour scheme with soft contrast

[3]: https://st.suckless.org/patches/delkey/ "Delete key"
[4]: https://st.suckless.org/patches/anysize/ "Anysize" 
[5]: https://st.suckless.org/patches/scrollback/ "Scrollback" 
[6]: https://st.suckless.org/patches/gruvbox/ "Gruvbox" 

### Configuration changes
> - Colors. Darker black for better contrast and to better blend in with the rest of my
>   system.

st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

