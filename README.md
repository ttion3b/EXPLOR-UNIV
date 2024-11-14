# EXPLOR-UNIV

!!!!!!!!!!!!!!!!!!!!!!!IMPORTANT!!!!!!!!!!!!!!!!!!!!!!!

Guide d'importation de la base de données avec phpMyAdmin
Prérequis :

1. Avoir une VM installée avec Apache2, PHP, et MariaDB.
2. phpMyAdmin doit être configuré et accessible sur la VM.
3. Le fichier universite.sql est prêt pour l'importation.

Étape 1 : Accéder à phpMyAdmin

1. Ouvrez un navigateur web sur votre VM ou sur un poste ayant accès à votre VM.

2. Allez à l’adresse suivante pour accéder à phpMyAdmin (remplacez localhost par l’IP de votre VM si besoin) :

http://localhost/phpmyadmin

3. Connectez-vous avec les identifiants suivants :

- Nom d'utilisateur : admin
- Mot de passe : admin

Étape 2 : Importer la base de données

1. Une fois connecté à phpMyAdmin, vous verrez une liste de bases de données sur le côté gauche.
2. Cliquez sur Nouvelle base de données en haut de la page (si vous n'avez pas encore de base de données appelée universite).
3. Donnez le nom universite à cette nouvelle base de données, puis cliquez sur Créer.
4. Une fois la base de données créée et sélectionnée, cliquez sur l'onglet Importer en haut de la page.
5. Dans la section Fichier à importer, cliquez sur Parcourir... et sélectionnez le fichier universite.sql depuis votre machine.
6. Vérifiez que le format est bien SQL, puis cliquez sur Exécuter en bas de la page pour lancer l'importation.

Étape 3 : Vérifier l'importation

Une fois l'importation terminée, un message de confirmation doit s'afficher. Vous pouvez maintenant vérifier que toutes les tables et données ont bien été importées en explorant la base de données universite dans phpMyAdmin.

Étape 4 : Déplacer le dossier "SITE"

Pour finir, placez le dossier SITE dans le répertoire des fichiers web d'Apache2 en utilisant cette commande (exécutée avec des droits sudo sur votre VM) :

sudo mv /chemin/vers/SITE /var/www/html/

Votre site est maintenant prêt à être consulté !
