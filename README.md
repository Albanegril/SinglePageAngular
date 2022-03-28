# Utiliser gitbhub page
Dans le cadre du cours de L3 informatique Architecture Logicielle Web

## Required

- avoir un repo github (privé éventuellement)
- avoir dans repository une application Angular fonctionnelle (qui peut build)

## Build une application angular

S'il n'y a pas d'erreur critique dans le code, l'application Angular pourra etre compilé : le TS n'est pas interprétable directement par le navigateur, il faut donc le traduire en JS.
La commande `ng serve` est utilisé durant la phase de développement.
La commande qui est utilisé lors de la mise en production de l'application est `ng build`,
Elle va créé une version compilé et executable de votre application, par défaut dans un dossier 'dist/' à la racine du projet

Ici on veut créer un nouveau dossier "docs" auquel pourra accéder github page, on précise donc un nouvel output-path (il peut aussi etre redéfinie directement dans `angular.json`)
`ng build --output-path ../docs --base-href /SinglePageAngular/`

Un 'Browser application bundle' est ainsi créé.

## Push le bundle

Il ne faut pas oublier de push le code dans le repository distant !

## Setup dans github

Il faut activé la fonctionnalité "pages",
Aller dans les `Settings` du projet, puis dans l'onglet `Pages`
Sélectionner une `source` (il est aussi possible d'avoir une branche dédié), par défaut la branche `main`, et le dossier "docs"

## Accéder à l'application

Dans cet exemple l'accès est à l'adresse : https://albanegril.github.io/SinglePageAngular/

## Visibilité

Attention, il faut noter que l'application une fois sur github page sera public, et ce quelque soit la visibilité initiale du projet !
