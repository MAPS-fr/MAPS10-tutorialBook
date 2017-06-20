# Comprendre et utiliser GIT

## Présentation

Git est un logiciel de gestion de version. Késako ?

Dixit ce [site web](https://git-scm.com/book/fr/v1/Démarrage-rapide-À-propos-de-la-gestion-de-version) qui offre de la documentation en libre accès sur git :

> Un gestionnaire de version est un système qui enregistre l'évolution d'un fichier ou d'un ensemble de fichiers au cours du temps de manière à ce qu'on puisse rappeler une version antérieure d'un fichier à tout moment.

Oui, en fait, de votre point de vue ça ressemble beaucoup à ce que fait Dropbox. A cette différence que git est capable de gérer le versionnement de vos fichiers à la ligne près. Le code de Linux \(+ 15 Millions de lignes\), ainsi que le code source d'autres millions de programmes, est géré sous git. L'autre grande différence c'est que git se manipule en utilisant des commandes. Toutefois et heureusement pour nous, il existe des **clients graphiques** qui facilite tout çà.

Comme Dropbox, Git va observer tout ce que vous faites dans un répertoire en particulier. On parle de **dépot**, ou de **repository** en anglais.

### Le fonctionnement théorique

Git fonctionne sur une architecture client serveur \(fig. 1\) qui permet aux utilisateurs de travailler conjointement dans un même projet. Si la modification peut se faire sur le même document, la procédure de validation des modification n'est pas évidente au premier arbord. Par contre le travail simultané sur différents document d'un même projet est particulièrement facile. 



![](/assets/schema_arch_server.png)

Figure 1 : fonctionnement de l'architecture

Pour chaque utilisateur le dépot GIT fonctionne de la même manière. On observe 3 espaces conceptuel : i\) un dossier de travail dans lequel sont sauvegarder les modification des différents fichiers, ii\) un espace d'index 

![](/assets/schema_arch_interne.png)



### Les commandes/mots-clefs

**Cloner un dépôt git** :

Lorsqu'on parle de recopier un **dépot** en ligne vers un ordinateur en local, on parle de **cloner** ce dépot.

La commande `git clone` permet de réaliser cette action.

```
git clone https://github.com/MAPS-fr/MAPS-10.git
```

**Ajouter des fichiers** :

Par défaut les nouveaux fichiers dans le dépôt ne sont pas suivis. Il faut faire la commande `git add nomdufichier` pour que git commence à suivre un fichier. Vous pouvez aussi demander à git de suivre tous les fichiers d'un répertoire en une fois avec la commande `git add .`

**Enregistrer l'état des modifications** :

`git commit`

** Récupérer les modifications du dépôt central** :

`git pull`

