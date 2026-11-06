# 🐧 QCM LINUX COMPLET - 50 QUESTIONS
## CCP3 - Exploiter des serveurs Linux

> **Durée conseillée** : 1h30  
> **Notation** : Chaque bonne réponse = 2 points (Total /100)  
> **Instructions** : Certaines questions peuvent avoir plusieurs bonnes réponses

---

## 📝 QUESTIONS

### PARTIE 1 - SYSTÈME DE FICHIERS (10 questions)

**Question 1** : Quel répertoire contient les fichiers de configuration système sous Linux ?
-  [ ] A) `/bin`
-  [V] B) `/etc`
-  [ ] C) `/var`
-  [ ] D) `/usr`

**Question 2** : Où se trouvent les fichiers des utilisateurs par défaut ?
-  [ ] A) `/root`
-  [V] B) `/home`
-  [ ] C) `/usr/home`
-  [ ] D) `/users`

**Question 3** : Quel fichier contient la liste des utilisateurs du système ?
-  [ ] A) `/etc/users`
-  [V] B) `/etc/passwd`
-  [ ] C) `/etc/shadow`
-  [ ] D) `/etc/group`

**Question 4** : Quel fichier contient les mots de passe chiffrés ?
-  [ ] A) `/etc/passwd`
-  [V] B) `/etc/shadow`
-  [ ] C) `/etc/secure`
-  [ ] D) `/etc/pwd`

**Question 5** : Quel répertoire contient les logs système ?
-  [ ] A) `/log`
-  [V] B) `/var/log`
-  [ ] C) `/sys/log`
-  [ ] D) `/etc/log`

**Question 6** : Quel fichier permet de configurer le montage automatique des partitions au démarrage ?
-  [ ] A) `/etc/mount`
-  [ ] B) `/etc/fstab`
-  [ ] C) `/etc/mtab`
-  [ ] D) `/boot/mount.conf`

**Question 7** : Quel répertoire contient les périphériques matériels ?
-  [ ] A) `/hardware`
-  [ ] B) `/devices`
-  [ ] C) `/dev`
-  [ ] D) `/sys`

**Question 8** : Où se trouve le fichier de configuration DNS ?
-  [ ] A) `/etc/dns.conf`
-  [V] B) `/etc/resolv.conf`
-  [ ] C) `/etc/network/dns`
-  [ ] D) `/var/dns/config`

**Question 9** : Quel fichier configure le serveur SSH ?
-  [ ] A) `/etc/ssh/ssh_config`
-  [V] B) `/etc/ssh/sshd_config`
-  [ ] C) `/etc/sshd.conf`
-  [ ] D) `/etc/ssh.conf`

**Question 10** : Quel répertoire contient les binaires essentiels du système ?
-  [ ] A) `/bin`
-  [ ] B) `/sbin`
-  [ ] C) `/usr/bin`
-  [ ] D) `/opt/bin`

---

### PARTIE 2 - GESTION UTILISATEURS ET GROUPES (10 questions)

**Question 11** : Quelle commande permet de créer un utilisateur avec son répertoire home ?
-  [ ] A) `useradd username`
-  [V] B) `useradd -m username`
-  [ ] C) `adduser username`
-  [ ] D) `create-user username`

**Question 12** : Comment ajouter un utilisateur à un groupe SANS écraser ses groupes actuels ?
-  [ ] A) `usermod -G groupe user`
-  [V] B) `usermod -aG groupe user`
-  [ ] C) `usermod -append groupe user`
-  [ ] D) `addgroup user groupe`

**Question 13** : Quelle commande permet de changer le mot de passe d'un utilisateur ?
-  [ ] A) `password username`
-  [ ] B) `passwd username`
-  [ ] C) `chpwd username`
-  [ ] D) `usermod -p username`

**Question 14** : Comment supprimer un utilisateur ET son répertoire home ?
-  [ ] A) `userdel username`
-  [ ] B) `userdel -r username`
-  [ ] C) `deluser username`
-  [ ] D) `rmuser -h username`

**Question 15** : Quelle commande affiche l'UID, le GID et les groupes d'un utilisateur ?
-  [ ] A) `whoami`
-  [ ] B) `id username`
-  [ ] C) `userinfo username`
-  [ ] D) `groups username`

**Question 16** : Comment créer un utilisateur avec un UID spécifique (1020) ?
-  [ ] A) `useradd -uid 1020 username`
-  [ ] B) `useradd -u 1020 username`
-  [ ] C) `useradd -id 1020 username`
-  [ ] D) `adduser --uid=1020 username`

**Question 17** : Quelle commande verrouille (désactive) un compte utilisateur ?
-  [ ] A) `usermod -L username`
-  [ ] B) `usermod -lock username`
-  [ ] C) `passwd -l username`
-  [ ] D) A et C sont correctes

**Question 18** : Comment créer un groupe avec un GID de 1050 ?
-  [ ] A) `groupadd -g 1050 nomgroupe`
-  [ ] B) `groupadd -gid 1050 nomgroupe`
-  [ ] C) `addgroup --gid 1050 nomgroupe`
-  [ ] D) `create-group -id 1050 nomgroupe`

**Question 19** : Quelle commande liste les utilisateurs actuellement connectés ?
-  [ ] A) `users`
-  [ ] B) `who`
-  [ ] C) `w`
-  [ ] D) B et C sont correctes

**Question 20** : Comment définir le shell d'un utilisateur à `/bin/bash` ?
-  [ ] A) `usermod -s /bin/bash username`
-  [ ] B) `chsh -s /bin/bash username`
-  [ ] C) `usermod --shell /bin/bash username`
-  [ ] D) A et C sont correctes

---

### PARTIE 3 - PERMISSIONS (10 questions)

**Question 21** : Que signifie la permission `rwxr-xr--` en octal ?
-  [ ] A) 755
-  [ ] B) 754
-  [ ] C) 644
-  [ ] D) 764

**Question 22** : Quelle commande donne tous les droits au propriétaire et aucun aux autres ?
-  [ ] A) `chmod 700 fichier`
-  [ ] B) `chmod 777 fichier`
-  [ ] C) `chmod 600 fichier`
-  [ ] D) `chmod u+rwx,go-rwx fichier`

**Question 23** : Comment ajouter le droit d'exécution pour tout le monde sur un fichier ?
-  [ ] A) `chmod +x fichier`
-  [ ] B) `chmod a+x fichier`
-  [ ] C) `chmod ugo+x fichier`
-  [ ] D) Toutes les réponses sont correctes

**Question 24** : Quelle commande change le propriétaire ET le groupe d'un fichier ?
-  [ ] A) `chown user fichier ; chgrp group fichier`
-  [ ] B) `chown user:group fichier`
-  [ ] C) `chown user.group fichier`
-  [ ] D) Toutes les réponses sont correctes

**Question 25** : Que signifie un umask de `0022` ?
-  [ ] A) Fichiers créés avec 644, dossiers avec 755
-  [ ] B) Fichiers créés avec 755, dossiers avec 777
-  [ ] C) Fichiers créés avec 666, dossiers avec 777
-  [ ] D) Fichiers créés avec 600, dossiers avec 700

**Question 26** : Comment appliquer récursivement les permissions 755 à un dossier et son contenu ?
-  [ ] A) `chmod 755 -r dossier`
-  [ ] B) `chmod -R 755 dossier`
-  [ ] C) `chmod --recursive 755 dossier`
-  [ ] D) B et C sont correctes

**Question 27** : Quelle valeur en octal correspond à `rw-rw-r--` ?
-  [ ] A) 664
-  [ ] B) 644
-  [ ] C) 744
-  [ ] D) 666

**Question 28** : Comment retirer le droit d'écriture au groupe sur un fichier ?
-  [ ] A) `chmod g-w fichier`
-  [ ] B) `chmod group-write fichier`
-  [ ] C) `chmod go-w fichier`
-  [ ] D) `chmod g=r fichier`

**Question 29** : Que fait la commande `chmod u+s fichier` ?
-  [ ] A) Ajoute le droit d'exécution
-  [ ] B) Applique le SUID (Set User ID)
-  [ ] C) Rend le fichier sticky
-  [ ] D) Rien, syntaxe incorrecte

**Question 30** : Comment changer récursivement le propriétaire d'un dossier ?
-  [ ] A) `chown -R user dossier`
-  [ ] B) `chown -r user dossier`
-  [ ] C) `chown --recursive user dossier`
-  [ ] D) A et C sont correctes

---

### PARTIE 4 - MANIPULATION DE FICHIERS (10 questions)

**Question 31** : Quelle commande affiche le contenu d'un fichier avec numérotation des lignes ?
-  [ ] A) `cat -n fichier`
-  [ ] B) `nl fichier`
-  [ ] C) `cat --line-numbers fichier`
-  [ ] D) A et B sont correctes

**Question 32** : Comment suivre un fichier de log en temps réel ?
-  [ ] A) `tail fichier`
-  [ ] B) `tail -f fichier`
-  [ ] C) `cat -f fichier`
-  [ ] D) `follow fichier`

**Question 33** : Quelle commande recherche les fichiers modifiés dans les 7 derniers jours ?
-  [ ] A) `find /chemin -mtime 7`
-  [ ] B) `find /chemin -mtime -7`
-  [ ] C) `find /chemin -modified 7d`
-  [ ] D) `find /chemin -recent 7`

**Question 34** : Comment rechercher le mot "error" dans un fichier (insensible à la casse) ?
-  [ ] A) `grep error fichier`
-  [ ] B) `grep -i error fichier`
-  [ ] C) `grep -ignore-case error fichier`
-  [ ] D) `grep --ignore-case error fichier`

**Question 35** : Quelle commande compte le nombre de lignes dans un fichier ?
-  [ ] A) `wc fichier`
-  [ ] B) `wc -l fichier`
-  [ ] C) `count fichier`
-  [ ] D) `lines fichier`

**Question 36** : Comment copier un dossier et tout son contenu ?
-  [ ] A) `cp dossier destination`
-  [ ] B) `cp -r dossier destination`
-  [ ] C) `cp -R dossier destination`
-  [ ] D) B et C sont correctes

**Question 37** : Que fait la commande `grep -v "texte" fichier` ?
-  [ ] A) Affiche les lignes contenant "texte"
-  [ ] B) Affiche les lignes NE contenant PAS "texte"
-  [ ] C) Compte les occurrences de "texte"
-  [ ] D) Recherche "texte" dans tous les fichiers

**Question 38** : Comment rediriger la sortie d'une commande en ajoutant à un fichier ?
-  [ ] A) `commande > fichier`
-  [ ] B) `commande >> fichier`
-  [ ] C) `commande >+ fichier`
-  [ ] D) `commande append fichier`

**Question 39** : Que fait le pipe `|` dans une commande ?
-  [ ] A) Redirige vers un fichier
-  [ ] B) Envoie la sortie d'une commande vers l'entrée d'une autre
-  [ ] C) Exécute deux commandes simultanément
-  [ ] D) Affiche les erreurs

**Question 40** : Comment rechercher tous les fichiers .conf dans /etc ?
-  [ ] A) `find /etc -name ".conf"`
-  [ ] B) `find /etc -name "*.conf"`
-  [ ] C) `locate /etc/*.conf`
-  [ ] D) `search /etc .conf`

---

### PARTIE 5 - RÉSEAU (10 questions)

**Question 41** : Quelle commande affiche la configuration réseau des interfaces ?
-  [ ] A) `ifconfig`
-  [ ] B) `ip addr show`
-  [ ] C) `ip a`
-  [ ] D) Toutes les réponses sont correctes

**Question 42** : Comment afficher la table de routage ?
-  [ ] A) `route -n`
-  [ ] B) `ip route show`
-  [ ] C) `netstat -r`
-  [ ] D) Toutes les réponses sont correctes

**Question 43** : Quelle commande teste la connectivité réseau vers une IP ?
-  [ ] A) `ping IP`
-  [ ] B) `test-connection IP`
-  [ ] C) `check IP`
-  [ ] D) `nettest IP`

**Question 44** : Comment afficher les ports en écoute avec netstat ?
-  [ ] A) `netstat -tuln`
-  [ ] B) `netstat -a`
-  [ ] C) `netstat -listening`
-  [ ] D) `netstat -ports`

**Question 45** : Quelle est l'alternative moderne à netstat ?
-  [ ] A) `ss`
-  [ ] B) `netcat`
-  [ ] C) `nstat`
-  [ ] D) `ipstat`

**Question 46** : Comment faire une résolution DNS avec dig ?
-  [ ] A) `dig domain.com`
-  [ ] B) `dig -query domain.com`
-  [ ] C) `resolve domain.com`
-  [ ] D) `dns-lookup domain.com`

**Question 47** : Sur Debian, quel fichier configure les interfaces réseau ?
-  [ ] A) `/etc/network/config`
-  [ ] B) `/etc/network/interfaces`
-  [ ] C) `/etc/interfaces`
-  [ ] D) `/etc/netplan/config.yaml`

**Question 48** : Comment activer une interface réseau ?
-  [ ] A) `ifup eth0`
-  [ ] B) `ip link set eth0 up`
-  [ ] C) `ifconfig eth0 up`
-  [ ] D) Toutes les réponses sont correctes

**Question 49** : Quelle commande trace la route des paquets vers une destination ?
-  [ ] A) `traceroute destination`
-  [ ] B) `tracepath destination`
-  [ ] C) `route-trace destination`
-  [ ] D) A et B sont correctes

**Question 50** : Comment changer le hostname de la machine ?
-  [ ] A) `hostname nouveau-nom`
-  [ ] B) `hostnamectl set-hostname nouveau-nom`
-  [ ] C) Modifier `/etc/hostname`
-  [ ] D) B et C sont correctes

---
