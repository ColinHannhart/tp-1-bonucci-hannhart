##TP 1 - Installation d’Ubuntu Server et prise
en main du shell

###Exercice 2. Prise en main de l’interpréteur de commandes
####Manuel
1) La commande Which localise une commande ou un binaire (commande faite : man which)
2) /option
3) On quitte le manuel en saisissant la commande q
4) La section 6 parle des differents petits jeux et programmes amusants présent dans le système d'exploitation

####Navigation dans l'arborescence des fichiers

1) Pour aller dans le dossier "/var/log", on tape la commande cd /var/log
2) Pour remonter dans le dossier parent "/var", on tape la commande cd..
3) Pour retourner dans le dossier personnel, on tape la commande cd
4) Pour revenir au dossier précédent, on tape la commande cd -
5) Lorsqu'on essaye d'accéder au dossier /root, la permission est refusée 
6) La commande sudo cd /root entraîne la demande d'un mot de passe pour accéder au dossier root
7) Pour créer l'arborescence décrite, on tape les commandes mkdir dossier1 dossier2 cd dossier1 touch fichier1 cd cd dossier2 mkdir dossier2 mkdir dossier2.1 dossier2.2 touch fichier2 fichier3 
8) Il n'est pas possible de supprimer le dossier
9) La commande qui permet de supprimer un dossier est rm -r
10) Même problème pour le dossier 2 il faut utiliser la commande rm -r
11) Il faut utiliser la commande rm -r pour supprimer un dossier et son contenu
###Exercice 3. Découverte de l’éditeur de texte nano
#### Commandes importantes
1) La commande qui permet d'afficher l'heure est la commande date. La commande time affiche l'usage des différentes ressources du système
2) Les fichiers commençant par un point sont des fichiers cachés 
3) Le programme ls se situe dans le dossier /bin/ls
4) La commande ll donne des informations sur les différents fichiers du dossier courant (date, propriétés...)
5) ls/bin
6) ls affiche les fichiers et dossiers du dossier courant ou spécifié
7) La commande pwd
8) Cette commande créer un fichier plop et écrit yo dedans
9) Cette commande créer un fichier plop et écrit yo dans le fichier 2 fois
10) Cette commande détermine le type d'un fichier
11)  Le contenu de toto est bien afficher dans titi, et titi n'est pas modifié lorsqu'on supprime toto
12) Si titi est modifié, tutu aussi et inversement. Si on supprime titi le lien se coupe et tutu devient inutilisable
13) CTRL+S pour stopper le défilement et CTRL+Q pour reprendre 
14) head - 5 /var/log/syslog pour les 5 premières lignes, Tail - 15 /var/log/syslog pour les 15 dernières lignes, 
head - 20 /var/log/syslog | tail - 10 pour les lignes 10 à 20
15) Affiche ce que fait le noyau page par page
16) Affiche les différents utilsateurs et groupe d'utilsateurs et masque les mot de passe
17) Cut -d : -f1 /etc/passwd | sort -r (-d)
18) Cut -d : -f1 /etc/passwd | sort -r | wc -l
19) man -k conversion | wc -l
20) find -name passwd
21) find -name passwd > /home/user/list_passwd_file.txt
find -name passwd 2> /dev/null
22) grep ll-r . -> ll dans le dossier .bashrc
23) history.log dans le dossier /var/log/apt/historylog
24) Non il n'apparaît pas car il faut d'abord mettre à jour la relevant database

###Exercice 4 : Personnalisation du shell
3) cp .bashrc ./.bashrc_back puis source_bashrc l'invite de cmd passe bien en couleur
4)
