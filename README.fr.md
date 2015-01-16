RKZen
=====

*(EN/FR project!)*

(L'outil bash qu'il vous faut pour flasher, sous Linux, une tablette Rockchip, tout en restant 'Zen' ...)

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

Vous trouverez les images officielles PIPO : http://www.pipo.cn/En/index.php?m=About&a=gujian

---

Pour l'instant, il n'est pas possible de flasher le Loader sous Linux, ni d'effectuer
 un 'Erase NAND(IDB)' ... affaire à suivre !

---

Installation
------------
Pré-requis :

° adb et fastboot : http://tablette-chinoise.net/faire-reconnaitre-sa-tablette-sous-linux-t3536
° rktools : https://github.com/rk3066/rk-tools
° rkflashtool: http://sourceforge.net/p/rkflashtool/Git/ci/master/tree/

1/ *[adb, fastboot]*<br />
    Suivre le tutoriel d'installation de ces outils pour faire reconnaître votre tablette, sous Linux

2/ *[rktools][2]*<br />
    Cliquez sur le bouton [ Download ZIP ] du dépôt GIT.<br />
    Une fois téléchargé, décompressez l'archive zip.<br />
    Dans une console terminal, dirigez-vous vers le répertoire décompressé, puis :<br />
    [code]<br />
    cd rk-tools<br />
    sudo apt-get install libssl-dev libcrypto++-dev<br />
    make<br />
    [/code]<br />
    Ceci installera les dépendances - librairies de développement - pour compiler
    les outils, puis compilera ceux-ci, pour créer les binaires nécessaires.<br />
    Une fois fait, vous devez découvrir les deux outils, principalement, nécessaires
     que sont 'afptool', 'img_unpack', ... verifiez !

3/ *[rkflashtool][3]*<br />
    NE PRENEZ PAS L'ARCHIVE 5.1 : il manque le fichier 'version.h' ... d'où le
    fait de prendre le snapshot GIT !!!<br />
    Cliquez sur le bouton [ Download Snapshot ] du dépôt GIT.<br />
    Une fois téléchargé, décompressez l'archive zip.<br />
    Dans une console terminal, dirigez-vous vers le répertoire décompressé, puis :<br />
    [code]<br />
    cd rkflashtool-master<br />
    sudo apt-get install libusb-1.0-0-dev<br />
    make<br />
    [/code]<br />
    Ceci compilera les binaires nécessaires, dont l'outil rkflashtool ...<br />
    Vérifiez qu'il n'y ait pas de message d'erreur !

[1]: See your distribution
[2]: https://github.com/rk3066/rk-tools
[3]: http://sourceforge.net/p/rkflashtool/Git/ci/master/tree/

Utilisation
-----------
1/ Assurez-vous que le script RK_Shell_Tools soit exécutable !
2/ IMPÉRATIF : lancez-le à partir d'une console terminal
3/ Répondez aux questions posées :p

Configuration
-------------
Il est possible d'utiliser un fichier de configuration pour faciliter un peu l'usage.<br />
Ouvrez le fichier 'config.readme' ; renseignez les valeurs nécessaires, puis
 enregistrez-le en tant que fichier 'config.ini' !<br />
 Si le fichier 'config.ini' existe certaines questions de configuration ne vous
 seront pas posées !<br />

Enjoy-it!
---------
"Allez, zou ... y'a plus qu'à ... !"


Forum
-----
Je peux certainement vous aider en français sur le forum de [Tablette Chinoise][1], ou en anglais sur celui de [FreakTab][2]!

[1]: http://tablette-chinoise.net/flasher-sa-rockchip-sous-linux-android-4-2-2-t4342
[2]: http://www.freaktab.com/showthread.php?10253-RKZen-Scripts-Bash-to-flash-under-Linux
