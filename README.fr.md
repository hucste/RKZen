RKZen
=====
(L'outil bash qu'il vous faut pour flasher, sous Linux, tout en restant 'Zen' ...)

Author
======
ATP : http://tablette-chinoise.net/membre4539.html
Dépôt GIT : https://github.com/hucste/RKZen

---

Vous trouverez les images officielles PIPO : http://www.pipo.cn/En/index.php?m=About&a=gujian

---

Pour l'instant, il n'est pas possible de flasher le Loader sous Linux, ni d'effectuer
 un 'Erase NAND(IDB)' ... affaire à suivre !

---

Installation
============

Pré-requis :

° adb et fastboot : http://tablette-chinoise.net/faire-reconnaitre-sa-tablette-sous-linux-t3536
° rktools : https://github.com/rk3066/rk-tools
° rkflashtool: http://sourceforge.net/p/rkflashtool/Git/ci/master/tree/

1/ adb et fastboot
    Suivre le tutoriel d'installation de ces outils pour faire reconnaître votre tablette, sous Linux

2/ rktools
    Cliquez sur le bouton [ Download ZIP ] du dépôt GIT.
    Une fois téléchargé, décompressez l'archive zip.
    Dans une console terminal, dirigez-vous vers le répertoire décompressé, puis :
    [code]
    cd rk-tools
    sudo apt-get install libssl-dev libcrypto++-dev
    make
    [/code]
    Ceci installera les dépendances - librairies de développement - pour compiler
    les outils, puis compilera ceux-ci, pour créer les binaires nécessaires.
    Une fois fait, vous devez découvrir les deux outils, principalement, nécessaires
     que sont 'afptool', 'img_unpack', ... verifiez !

3/ rkflashtool
    NE PRENEZ PAS L'ARCHIVE 5.1 : il manque le fichier 'version.h' ... d'où le
    fait de prendre le snapshot GIT !!!
    Cliquez sur le bouton [ Download Snapshot ] du dépôt GIT.
    Une fois téléchargé, décompressez l'archive zip.
    Dans une console terminal, dirigez-vous vers le répertoire décompressé, puis :
    [code]
    make
    [/code]
    Ceci compilera les binaires nécessaires, dont l'outil rkflashtool ...
    Vérifiez qu'il n'y ait pas de message d'erreur !

*** *********************************************************************** ***
*** Petit bonus, vous trouverez les archives zip 'rktools' et 'rkflashtool'
***  dans le répertoire 'tools', dans l'archive zip ! (archives du 23/01/2014).
*** Préférez les décompresser dans ledit répertoire, puis compilez-les !
*** *********************************************************************** ***

Utilisation
===========

1/ Assurez-vous que le script RK_Shell_Tools soit exécutable !
2/ IMPÉRATIF : lancez-le à partir d'une console terminal
3/ Répondez aux questions posées :p

Configuration
=============
Il est possible d'utiliser un fichier de configuration pour faciliter un peu l'usage.
Ouvrez le fichier 'config.readme' ; renseignez les valeurs nécessaires, puis
 enregistrez-le en tant que fichier 'config.ini' !
 Si le fichier 'config.ini' existe certaines questions de configuration ne vous
 seront pas posées !

Enjoy-it!
=========
Allez, zou ... y'a plus qu'à ... !

Auteur
======
ATP : http://tablette-chinoise.net/membre4539.html
