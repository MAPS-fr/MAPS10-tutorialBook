
Remarques : les éléments entre **$$**, comme **$VOTRENOM$** doivent être adapté par vos soins pour votre ordinateur.

## Le modèle Netlogo

 Le répertoire sous Windows qui correspond à vos document est le suivant : `C:\Users\$VOTRENOM$\Documents\` 

Dans ce répertoire nous allons créer un dossier "**Repository**" qui contiendra le dépot git de notre modèle. Attention à la majuscule...

## Créer un repository git 

Lancer le logiciel SourceTree qui sert de client graphique pour le programme git. Normalement vous devez déjà avoir configuré le logiciel pour fonctionner avec GitHub. Si ce n'est pas le cas faite d'abord la partie [prérequis](../prerequis.md).

Dans la barre de menu, cliquez sur l'onglet **Create** qui permet d'initialiser un nouveau depot git vide : 

![](/assets/2017-06-16 22_19_36-SourceTree.jpg)

SourceTree va créer un nouveau dépot "**monModeleMaps**" dans `C:\Users\$VOTRENOM$\Documents\Repository\` et le relier à votre compte utilisateur GitHub **[Repository Settings]** lorsque vous allez appuyer sur le bouton **[Créer]**.

Des informations vous sont demandées, elles serviront à identifier les modifications par la suite.

![](/assets/2017-06-16 22_21_22-SourceTree.jpg)

Après création, voici l'interface de gestion de votre dépot git.  

![](/assets/2017-06-16 22_25_10-SourceTree.jpg)# Updloader votre modèle sur GitHub

Le dépot git vide apparait en local dans `C:\Users\$VOTRENOM$\Documents\Repository\monModeleMaps` et en ligne sur github à l'url suivante **https://github.com/$VOTRELOGINGITHUB$/monModeleMaps**

Comme vous le voyez il n'y a rien.
 
A nouveau dans **SourceTree**, cliquez sur le petit **+** pour ouvrir un nouvel onglet.

![](/assets/2017-06-16 22_27_37-SourceTree.jpg)

A tout moment vous pouvez voir les dépot git en local en cliquant sur l'icone **[Local]** dans la barre, et les dépot git en ligne en cliquant sur l'icone **[Remote]**

![](/assets/2017-06-16 22_30_51-SourceTree.jpg)

Nous allons à présent **ajouter des fichiers** à notre nouveau dépot.

## Ajout du modèle Netlogo au dépot

Télécharger le [zip suivant](assets/modeleMaps.zip) , qui contient le modele `ants.nlogo`, et décompresser le. Faite ensuite glisser les fichiers `Ants.nlogo` et `Ants.png` dans notre dépot `C:\Users\$VOTRENOM$\Documents\Repository\monModeleMaps`

Si vous revenez dans l'onglet **monModeleMaps** vous verrez que les fichiers sont apparus dans la fenêtre du bas. Comme ce sont de nouveau fichier, **SourceTree** nous indique qu'il ne sont pas encore indexé par git, ce qui est le comportement par défaut.

![](/assets/2017-06-16 22_34_16-SourceTree.jpg) 
  
Cliquez sur le bouton **[ToutIndexer]** pour que git commence à suivre les modifications sur ces fichiers. Comme vous le voyez les fichiers passe dans la zone du haut.

![](/assets/2017-06-16 22_39_43-SourceTree.jpg)

Validons ce nouvel état du dépot. Pour cela il suffit de rentrer un message dans la fenetre du bas, qui sert à indiquer aux autres utilisateurs du dépot les modifications que nous avons faites sur le modèle. Dans le cas présent nous avons juste ajouter des fichiers.

![](/assets/2017-06-16 22_43_11-SourceTree.jpg)

 Cliquez ensuite sur **[valider]** (ce qui correspond à la commande `commit `dans git) pour voir ce qu'il se passe. De nouveau **SourceTree** qu'il n'y a plus rien à valider. Pour le moment nous avons juste travailler en local, cliquez sur la flèche **[envoyer]** du bandeau pour envoyer les modifications que nous venons de faire sur GitHub. Une fenetre s'ouvre, cochez la case dans la colonne **[Envoyer]** puis cliquez sur le bouton **[Envoyer]**
 
 ![](/assets/2017-06-16 22_46_58-SourceTree.jpg)

Si vous retournez voir votre dépot en ligne sur le site GitHub, celle-ci a été mise à jour.

![](/assets/2017-06-16 22_49_47-reyman_monModeleMaps.jpg)

## Suivi des modifications

Faisons une modifications dans le fichier `Ants.nlogo` pour voir ce qu'il se passe dans SourceTree. 

Comme vous pouvez le voir sur l'image ci-dessous, git a detecté que j'ai modifié la taille et la couleur des fourmis. En rouge apparait ce qui a été supprimé, et en vert ce qui a été ajouté.

![](/assets/2017-06-16 22_51_47-SourceTree.jpg)

Pour valider ces modifications, il faut à nouveau **[indexer]** le fichier, puis le **[valider]** en écrivant un message explicatif.

Si vous cliquez sur la droite sur l'icone **[BRANCHES]**, puis **[master]** vous pouvez observer l'historique du projet, avec, ce qui est important, la possibilité de visionner les modifications en cliquant sur les différentes lignes. Il est également possible de revenir en arrière, mais nous en parlerons ensuite.

![](/assets/2017-06-16 22_59_25-SourceTree.jpg)

Si nous nous intéressons aux deux lignes suivantes, l'état du dépot local est indiqué par l'icone [master], et l'état du dépot en ligne par l'icone [origin/master]. 

![](/assets/2017-06-16 23_02_13-SourceTree.jpg)

Comme vous vous en doutiez, l'état local est en effet en avance sur le dépot central, cliquons sur **[envoyer]** pour synchroniser les deux dépots, comme ci dessous. Vous pouvez regarder en ligne sur github pour vérifier.

![](/assets/2017-06-16 23_06_00-SourceTree.jpg)

## Partager votre dépot

Aller sur l'url de votre modèle github **https://github.com/$VOTRELOGINGITHUB$/monModeleMaps** et cliquez sur le bouton clone or download.

![](/assets/2017-06-16 23_27_46-reyman_monModeleMaps.jpg) 

Vous pouvez partager l'url en https qui apparait (**https://github.com/$VOTRELOGINGITHUB$/monModeleMaps.git**) avec votre voisin qui va à présent tenter de cloner votre dépot sur son ordinateur et d'ajouter un fichier README.md

## Cloner et modifier un dépot existant en ligne

Dans **SourceTree**, cliquez sur l'icone **[Clone]**

![](/assets/2017-06-16 23_31_23-SourceTree.jpg)

Entrez l'adresse git https qui vous a été donné par votre voisin, et indiquez l'endroit ou vous voulez que soit cloner le dépot en ligne sur votre ordinateur. Nous choisissons de le mettre dans le même répertoire **Repository**, sous le nom **modeleDeMonVoisin** (Attention, le dossier ne doit pas exister !!) 

![](/assets/2017-06-16 23_39_12-SourceTree.jpg)

Appuyez ensuite sur le bouton **[Cloner]**

Comme vous pouvez le constater, un nouveau dossier est apparu dans votre arborescence : 

![](/assets/2017-06-16 23_42_38-Repository.jpg)

Nous allons rajouter un fichier `README.md` à ce dépot **modeleDeMonVoisin**. Ce fichier est automatiquement affiché en page d'accueil du dépot lorsqu'on se rend sur l'url du site, c'est pratique par exemple pour mettre de la documentation. Ajouter ce texte au fichier `README.md` : 

```
#Documentation
Ouvrir le fichier .nlogo avec Netlogo 6.1
```

Revenez dans SourceTree, à l'onglet **modeleDeMonVoisin**. Comme vu précédemment, **[Indexer]** le fichier, ajouter un message dans le formulaire en bas, et **[Valider]**.

![](/assets/2017-06-16 23_50_13-SourceTree.jpg)

# Récupérer des modifications faites sur le dépot en ligne

Nous allons maintenant tenter de recupérer les modifications faites par votre voisin sur votre projet. Pour cela revenez dans l'onglet **monModeleMaps** et cliquer sur l'icone **[Récupérer]**.

![](/assets/2017-06-16 23_52_45-SourceTree.jpg)

Une fenetre s'ouvre, faite simplement **[Ok]**

![](/assets/2017-06-16 23_54_03-(modified) Créer, modifier et publier un dépot git — GitBook Editor.jpg)

Voilà, nous avons récupérer les modifications faites par votre voisin ! Vous pouvez consulter l'url du dépot sur github pour voir l'affichage du `README.md`






