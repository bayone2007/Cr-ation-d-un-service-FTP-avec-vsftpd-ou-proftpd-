# Cr-ation-d-un-service-FTP-avec-vsftpd-ou-proftpd-
1. Présentation du projet
   Notre travail porte sur la création d’un serveur FTP (file transfert protocol) avec vsftpd (very security file transfert protocol daemon) et proftpd ( professional  file transfert protocol daemon).Ce projet consiste à déployer, créer, modifier et sécuriser un serveur qui permet le transfère des fichiers entre plusieurs machines, ces fichiers peuvent être téléchargés et peuvent être gérer à distance. L’objectif est de fournir une solution permettant le partage des fichiers tout en garantissant l’intégrité et la confidentialité des données.les différentes échanges peuvent être réaliser entre le client (FileZilla, navigateur, terminal, …) et un serveur (ordinateur, serveur Linux, …).
Ce projet nous permet de :
  - Partager des fichiers à distance entre plusieurs machines et pouvoir y accéder .
  - Centraliser les données et comprendre le fonctionnement d’un serveur.
  -  Apprendre l’administration du système Linux.
     Ex : - Une entreprise  qui partage des documents en internes         - Un administrateur qui sauvegarde des fichiers à distance        - Un étudiant transfère des fichiers à distance entre un PC et téléphone.
      Pour ces différentes situation, vsftpd et proftpd sont justement le meilleur choix possible.
     Pour la création d’un serveur simple, stable, léger et sécurisé vsftpd est idéal.
2. Architecture et technologies      Système d’exploitation utilisé : Linux( distribution Ubuntu) via VMWareserveur
FTP principal : vsftpd
outils de test : Filezilla
FTP CLI : client en ligne de commande sur le terminal
Nmap & Hydra : Tests de sécurité et d’intrusion
3. Installation et configuration
a. Installation de vsftpd :               sudo apt update
      sudo apt install vsftpd
b. Vérification du fonctionnement du serveur :
      sudo systemctl status vsftpd (s’il est activé on aura run:Actived)
sinon :
      sudo systemctl start vsftpd         sudo systemctl enablevsftpd
c. Creer un utilisateur FTP :             sudo adduser ftpuser
d. Le fichier de configuration principal de vsftpd(/etc/vsftpd.conf)                Dans le fichier principal de configuration nous avons eu à appliquer une politique de sécurité qui est la suivante :
- Local_enable=YES : autorise aux utilisateurs locaux de se connecter au servveur
- Write_enable=YES : Permet l’écriture sur le serveur
- Anonymous_enable=YES : Accès anonyme limité à la lecture seulement
- Chroot_local_user=YES : Evite toute navigation non autoriséé dans le serveur en emprisonnant les utilisateurs dans leur repertoire personnel.
  4. Les membres du groupe 21
     1.MBOLI MOSENGO PHRASIA
     2.BAYONE PHAMBU JEREMI
     3.ANGESAKA WINNER WINNER
     4.MUTOKETUKUTSHUJESSICA
     5.MOKULAYANGA MAYENA DIVINA
     6.LUAM’NSA BIN LUAMBO AGRADI        7.NSITUVUIDI KAPITA PLADI
     8.TSHIBUNGU BULANDAJASON
     9.MWAMBA MUTOMBO TYCHIQUE
     10.TABI  DUMBI CHRISTOPHER      
