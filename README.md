RKZen
=====

*(EN/FR project!)*

Scripts Bash to flash Rockchip tablet under Linux.

Author
------

**HUC Stéphane** : <devs@stephane-huc.net><br />
*alias* : *ATP* : [FreakTab][2],[Tablette Chinoise][1], 
[1]: http://tablette-chinoise.net/membre4539.html
[2]: http://www.freaktab.com/member.php?42437-ATP
<br />
*GIT* : https://github.com/hucste/RKZen<br />
*Licence* : CC0 http://directory.fsf.org/wiki/License:CC0

---

You will find Officials ROM PIPO : http://www.pipo.cn/En/index.php?m=About&a=gujian

----

@the time, it's not possible to flash RKLoader*.bin, erase NAND (IDB) under Linux.
 It's always necessary to use MS Windows plateform with tool as RKAndroidTool!

----

This tool need others tools :

1/ *[adb, fastboot][1]*<br />
    For *Buntu 13.04 >= (and like), use PPA:
    https://launchpad.net/~phablet-team/+archive/tools
    For Debian Wheezy: use backports repository... 
    For Debian Jessie, or Sid: use native repository

2/ *[rktools][2]*<br />
    Click on button [ Download ZIP ] onto website GIT.<br />
    Uncompress the archive zip<br />
    In terminal, go to the archive uncompressed directory, and:
    [code]
    cd rk-tools
    sudo apt-get install libssl-dev libcrypto++-dev
    make
    [/code]<br />
    This install development libraries needed, and compil rktools.
    Verify if error message.

3/ *[rkflashtool][3]*<br />
    DON'T DL ARCHIVE 5.1: the file 'version.h' is forgotten.<br />
    Click on button [ Download Snapshot ] onto website GIT.<br />
    Uncompress the archive zip<br />
    In terminal, go to the archive uncompressed directory, and:
    [code]
    cd rkflashtool-master
    sudo apt-get install libusb-1.0-0-dev
    make
    [/code]
    This compil tools needed.<br />
    Verify if error message.

[1]: See your distribution
[2]: https://github.com/rk3066/rk-tools
[3]: http://sourceforge.net/p/rkflashtool/Git/ci/master/tree/

---

USE
---
1/ make script RK_Shell_Tools executable!<br />
2/ IMPERATIVE: run-it in terminal-console.<br />
3/ answer questions :p<br />

Config
------
It's possible to use file config.<br />
Open file 'config.readme'; write the values needed and save as 'config.ini'.<br />
If file 'config.ini' isn't exists, the RK_Shell_Tools will ask you some questions.<br />

Enjoy-it!
---------
!!! It's still into development !!! <br />
!!! Use at yours personals risks !!!

Forum
-----
I can help you sometimes, asap, in French onto [Tablette Chinoise][1], or in English onto [FreakTab][2]!

[1]: http://tablette-chinoise.net/flasher-sa-rockchip-sous-linux-android-4-2-2-t4342
[2]: http://www.freaktab.com/showthread.php?10253-RKZen-Scripts-Bash-to-flash-under-Linux

