RKZen
=====

(French project!)

Scripts Bash to flash Rockchip tablet under Linux.

Author
======
ATP : http://tablette-chinoise.net/membre4539.html
GIT : https://github.com/hucste/RKZen

----
@the time, it's not possible to flash RKLoader*.bin, erase NAND (IDB) under Linux.
 It's always necessary to use MS Windows plateform with tool as RKAndroidTool!

----

This tool need others tools :

- adb 'n fastboot: Please see your distribution Linux.
- rkflashtool: https://github.com/rk3066/rk-tools
- rktools: http://sourceforge.net/p/rkflashtool/Git/ci/master/tree/

1/ adb, fastboot
    For *Buntu 13.04 >= (and like), use PPA:
    https://launchpad.net/~phablet-team/+archive/tools

2/ rktools
    Click on button [ Download ZIP ] onto website GIT.
    Uncompress the archive zip
    In terminal, go to the archive uncompressed directory, and:
    [code]
    cd rk-tools
    sudo apt-get install libssl-dev libcrypto++-dev
    make
    [/code]
    This install development libraries needed, and compil rktools.
    Verify if error message.

3/ rkflashtool
    DON'T DL ARCHIVE 5.1: the file 'version.h' is forgotten.
    Click on button [ Download Snapshot ] onto website GIT.
    Uncompress the archive zip
    In terminal, go to the archive uncompressed directory, and:
    [code]
    make
    [/code]
    This compil tools needed.
    Verify if error message.

---

USE
====
1/ make script RK_Shell_Tools executable!
2/ IMPERATIVE: run-it in terminal-console.
3/ answer questions :p

Config
======
It's possible to use file config.
Open file 'config.readme'; write the values needed and save as 'config.ini'.
If file 'config.ini' isn't exists, the RK_Shell_Tools will ask you some questions.

Enjoy-it!
=========
