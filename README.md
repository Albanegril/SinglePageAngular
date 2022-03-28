# SinglePageAngular
Dans le cadre du cours de L3 informatique Architecture Logicielle Web

## Use gitbhub page

### Required

- avoir un repo github (privé éventuellement)
- avoir dans ce premier repository une application Angular fonctionnel (qui peut build)

### Build une application angular

S'il n'y a pas d'erreur critique dans le code, l'application Angular pourra etre compilé : le TS n'est pas interprétable directement par le navigateur, il faut donc le traduire en JS.
La commande `ng serve` est utilisé durant la phase de développement.
La commande qui est utilisé lors de la mise en production de l'application est `ng build`,
Elle va créé une version compilé et executable de votre application, par défaut dans un dossier 'dist/' à la racine du projet

Un 'Browser application bundle' est ainsi créé

### Créé un projet publique

Afin de rendre le projet accessible il faut créé un nouveau repository dans github, dont le nom sera utilisé dans l'url d'accès (autant que se soit le nom de l'application).
Ce projet doit pour le moment rester vite, éventuellement avec un README,
Il est ensuite cloné en local, à coté du repository de travail précédent.

### Mettre le bundle de application dans le repo public

Cette étape peut ce faire de 2 façon différentes :

il est possible de copier/coller le bundle créé avec `ng build` dans le nouveau repo public créé en local,

il est également possible de modifier le 'outputPath' de build dans le file 'angular.json', ainsi de "dist/dashfront" il deviendra "../../SinglePageAngularPublic/dashfront" dans mon exemple.

### Push le bundle

Se rendre dans le repo git public (dans lequel est le bundle) et push le contenu nouvellement ajouté

### Setup dans github

Une fois le code ajouté au repo distant (dans github), il faut activé la fonctionnalité "pages",
Aller dans les 'Settings' du projet, puis dans l'onglet 'Pages'
Selectionner une source (il est aussi possible d'avoir une branche dédié au lieu d'un repo différent)

### Accéder à l'application

dans cet exemple l'accès est à l'adresse : https://albanegril.github.io/SinglePageAngularPublic/
