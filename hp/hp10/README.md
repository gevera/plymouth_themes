hp10 Plymouth Theme
=======================

HP à la Windows 10 boot splash theme for Plymouth


Based on

- Pure CSS Windows10 Loader by Fernando de Almeida Faria  
  https://codepen.io/feebaa/pen/PPrLQP
- Deb10 by Mauro A. Meloni <maumeloni@gmail.com>
and
- Plymouth theming guide (part 4)  
  http://brej.org/blog/?p=238

Documentation about scripting available at
- https://www.freedesktop.org/wiki/Software/Plymouth/Scripts/
and
- https://sources.debian.org/src/plymouth/0.9.2-4/src/plugins/splash/script/

## Installation

**Step 1**
Untar the downloaded archive file

    tar xvaf hp10.tar.gz

**Step 2**
Copy *hp10* folder to */usr/share/plymouth/themes*
### Option 1
Manually 

    sudo cp -vr hp10 /usr/share/plymouth/themes/

### Option 2
Or automatically. To do that you need to change directory to the archive folder   
      
    cd hp10

Run following command to copy theme folder automatically to */usr/share/plymouth/themes*

    make install   # as root or with sudo

To make sure that the theme is indeed installed execute

    sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/hp10/hp10.plymouth 100

Choose the *hp10* theme to be activated

    sudo update-alternatives --config default.plymouth

Update initramfs

    sudo update-initramfs -u       

Reboot to see the new theme

    reboot

### License

This theme is licensed under GPLv2, for more details check COPYING.
