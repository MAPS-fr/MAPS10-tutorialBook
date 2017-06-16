
# Github et Git, quelques mots de présentation

## Git

### Présentation 

Git est un logiciel de gestion de version. Késako ? 

Dixit ce [site web](https://git-scm.com/book/fr/v1/D%C3%A9marrage-rapide-%C3%80-propos-de-la-gestion-de-version) qui offre de la documentation en libre accès sur git : 
> Un gestionnaire de version est un système qui enregistre l'évolution d'un fichier ou d'un ensemble de fichiers au cours du temps de manière à ce qu'on puisse rappeler une version antérieure d'un fichier à tout moment. 

Oui, en fait, de votre point de vue ça ressemble beaucoup à ce que fait Dropbox. A cette différence que git est capable de gérer le versionnement de vos fichiers à la ligne près. Le code de Linux (+ 15 Millions de lignes), ainsi que le code source d'autres millions de programmes, est géré sous git. L'autre grande différence c'est que git se manipule en utilisant des commandes. Toutefois et heureusement pour nous, il existe des **clients graphiques** qui facilite tout çà.

Comme Dropbox, Git va observer tout ce que vous faites dans un répertoire en particulier. On parle de **dépot**, ou de **repository** en anglais.



### Les commandes/mots-clefs

Lorsqu'on parle de recopier un **dépot** en ligne vers un ordinateur en local, on parle de **cloner** ce dépot. La commande `git clone` permet de réaliser cette action.

```
git clone https://github.com/MAPS-fr/MAPS-10.git
```


## Github

### Présentation rapide

GitHub est tout simplement un site web qui permet de déposer vos dépots git sur Internet. Il en existe d'autres (gitlab, gog, etc.), mais github est **le premier et le plus gros hub de partage de code source** dans le monde. 

Il y a deux niveaux d'organisation, les dépots peuvent être créés ou déposé sous la bannière d'utilisateur, ou d'organisations (qui contiennent des utilisateurs). 

L'organisation MAPS par exemple regroupe plusieurs dépots avec les modèles et les supports de présentations des années précédentes : https://github.com/MAPS-fr Certains laboratoires dispose dejà de leur organisation sur github, comme l'[UMR Géographie-cités](https://github.com/Geographie-cites), ou l'[UMR IDEES](https://github.com/IDEES-Rouen). C'est une façon simple d'organiser et de valoriser les productions logicielles des chercheurs.

Github est gratuit pour les codes sources qui sont publics, et donc open-source. Si vous souhaitez que vos dépots soit privés, alors il vous faudra dépenser un peu d'argent pour un abonnement.

### Fonctionnement

Dans tous les cas il faut comprendre que le dépot local (votre ordinateur) et le dépot en ligne (github, ou autre site) sont liés entre eux. Toutes les personnes qui ont cloné un dépot en ligne sur leur ordinateur local peuvent modifier les fichiers et ensuite renvoyer les modification au dépot en ligne. Github permet d'organiser et de centraliser ces échanges de versions entre développeurs. C'est donc aussi un peu un réseau social pour développeur.

Il faut bien noter que la synchronisation entre un dépot en ligne et un dépot local ne se fait pas automatiquement comme dans le cas de Dropbox. Chaque utilisateur va devoir taper des commandes (dans un terminal) ou cliquer sur des boutons (si on est dans une interface graphique)

Dans github vous avez deux possibilités : 
- créer un dépot en ligne via github, et ensuite le cloner sur votre ordinateur
- créer un dépot sur votre ordinateur et ensuite l'envoyer sur github
 


# Créer un compte Github

Rien de plus simple, il suffit d'aller sur le site https://github.com/






