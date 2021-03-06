# Symfony 4.2 Jobeet Project

### Pour un travail en local : 
**Prérequis :**
* Installation de composer : https://getcomposer.org/ 
* Installer Git : https://git-scm.com/ 
* Installer PHP 7.1 + MySQL + apache : 
https://www.wampserver.com/ 
https://www.uwamp.com/fr/ 
https://doc.ubuntu-fr.org/lamp 


### Vous pouvez au choix utiliser un hébergeur si vous le souhaitez.


### Importer le projet :
Git clone : https://github.com/webcontrat/jobeet_remy


### Installer le projet :

    composer install

Modifier dans le .env la configuration de l’accès à la  base de données : DATABASE_URL

    php bin/console doctrine:migration:migrate
    php bin/console doctrine:fixtures:load 
    php bin/console server:start

### Information sur l’application Jobeet :
Accès à l’admin : /login

User : admin
Password : admin

 
#### Fonctionnalité à développer : 
Jobeet est une application permettant de gérer des offres d’emploi.

Le but de la fonctionnalité à développer est de pouvoir postuler à une offre d’emploi de manière très simplifiée.

Pour cela, il faudra rajouter un bouton sur l'offre pour pouvoir y postuler :

Ce bouton doit mener à un formulaire avec les champs suivants à remplir par l’utilisateur :
 * Nom (champ obligatoire)
 * Prénom (champ obligatoire)
 * Mail (champ obligatoire)
 * Numéro de téléphone
 * Adresse

Il faut enregistrer automatiquement la date à laquelle l’utilisateur a postulé à l’emploi. Cette postulation doit être liée à l’offre d’emploi dans la base de données.

Les données doivent être enregistrées dans une nouvelle table que vous aurez créée au préalable.

Pour finir, vous devrez afficher la liste des postulants dans la section « Administration » du site.

Merci de ne développer que ce qui est indiqué au-dessus, les autres développements ne seront pas pris en compte.


### Nous retourner votre développement :

Merci de commit votre code sur une nouvelle branche (pas la master).

Ensuite de creer une pull request de votre branche vers la master. Ne pas la valider. Nous aurons ainsi en visuel les modifications que vous avez effectuez. Votre pull request devra être effectué avant le dimanche 6 septembre à minuit.

[Documentation GIT](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests)


### Documentation :

Pour vous aider voici le tutoriel jobeet, ne pas suivre les indications du jour 1 (Jobeet Day 1: Starting up the Project).

Tutorial: [https://github.com/gregurco/jobeet-tutorial][1]

[1]: https://github.com/gregurco/jobeet-tutorial
