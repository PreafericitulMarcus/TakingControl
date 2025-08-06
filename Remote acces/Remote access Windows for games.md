Remote access Windows for games
========================

Roadmap:

### Change boot option ( I dual boot Ubuntu Server and Windows 10 );

1. Identify OS Boot Entry:

```
    sudo grep menuentry /boot/grub/grub.cfg

    mentuentry 'Ubuntu' ...
    mentuentry 'Windows Boot Manager (on dev/sdX)' ...
```

2. Boot into windows after reboot with ( [GRUB](https://wiki.debian.org/GrubReboot) ) (tl;dr GRUB contains the ability to reboot into a specified menuentry **once.**)

*replace sdX with your partition ( use **lsblk** to find  )*
```
    sudo grub-reboot "Windows Boot Manager (on /dev/sdX)"
    sudo reboot
```

Wait a bit.  And you should be in Windows.

I use Parsec in order to play games.

When you finish your Windows session just restart and you will be back on Ubuntu Server.

For an easier time i created a script "changeWindows.sh" with

```
    #!/bin/bash
    
    sudo grub-reboot "windows Boot Manager (on /dev/sdX)" #change here sdX with your partition.
    sudo reboot
```
Save and change permission:
```
    chmod u+x changeWindows.sh
```
<br>


###  Parsec and/or Sunshine + Moonlight + Tailscale

In order to actually access the content I need either Parsec which is a lot easier to set up but it is not open source. Or the other option which I read is faster for games. 

For just a casual remote use of a computer Parsec is definitely the best.

To set up Parsec you just [download](https://parsec.app/downloads) on both the Host and Client, Log in and enjoy.

The other method is to:
[Download Sunshine](https://github.com/LizardByte/Sunshine?tab=readme-ov-file) on Host machine ( Windows in my case ).<br>
[Download Moonlight](https://github.com/moonlight-stream/moonlight-qt) on Client.<br>
Optional: If you want to remote access outside local network<br> 
[Download Tailscale](https://tailscale.com/download)


I use both option just in case one fails, but also test which I like more. 
