+++
title = "Tour de Hanoi en Java Swing"
menuTitle = "TP3 - Tour de Hanoi"
draft = false
weight = 30
+++

Le troisième projet est la création d'une application avec les librairies graphiques de Java Swing.

Le projet sera découpé en deux parties:

* La conception de l'interface
* L'ajout d'interactions dans l'interface

### Instructions

* En équipe de deux ou trois.
* Étudiez les méthodes des classes fournies pour bien comprendre leurs fonctionnements.
* Implémentez les classes demandées en vous basant sur la documentation fournie.
* Remise sur Moodle le 16 juillet avant 23h59.

### Description de l'application

Nous voulons faire une application qui nous permet de jouer au jeu des [Tours de Hanoï](https://fr.wikipedia.org/wiki/Tours_de_Hano%C3%AF). Le jeu consiste à avoir 3 tours avec des disques placés en ordre de taille débutant sur un des tours. Le but du jeu est de déplacer tous les disques sur une autre tour en respectant les règles suivantes :

* On déplace un seul disque à la fois.
* On ne peut pas placer un disque sur un disque plus petit.

Il est possible de voir une implémentation du jeu pour se familiariser avec ses règles [à l'adresse suivante](https://www.mathsisfun.com/games/towerofhanoi.html).

## Partie 1 - Conception de l'application

Nous voulons avoir une application qui nous permet de jouer au jeu des tours de Hanoi. L'application finale doit ressembler à ceci :

![table](/INF111/images/TP3/hanoiSwing.png?width=40pc)

### Listes des éléments de l'application

### Tour de Hanoi en JComponent

![table](/INF111/images/TP3/HanoiTowerComponent.png?width=20pc)

**Ce composant vous est fourni** dans une version simple pour la partie 1.
Il représente une des tours de Hanoï.

* Type : JComponent
* Taille : 200 * 350

Téléchargé [ici](/TP3/HanoiTowerComponent.java)

### Tour de Hanoï avec bouton

![table](/INF111/images/TP3/HanoiTowerPanel.png?width=20pc)

Ce panel va inclure le composant de la tour de Hanoi avec un bouton pour sélectionner la tour.

* Type : JPanel
* Taille : 200 * 350
* Layout : BoxLayout en Y

### Liste des tours de Hanoï

![table](/INF111/images/TP3/HanoiTowerListPanel.png?width=30pc)

Ce panel va contenir les 3 tours de Hanoï de notre jeu avec leurs boutons respectifs.

* Type : JPanel
* Taille : 600 * 350
* Layout : BoxLayout en X

### Panneau supérieur de sélection de disques

![table](/INF111/images/TP3/HanoiTopPanel.png?width=30pc)

Ce panel va conserver l'information du disque sélectionné qui pourra bouger entre les tours.

* Type : JPanel
* Taille : 600 * 100
* Layout : BoxLayout en X

L'affichage du disque vous est fourni dans une classe de type JComponent. Cette classe aura plus de fonctionnalité durant la deuxième partie.

Vous pouvez trouver la classe du composant du disque [ici](/TP3/HanoiRingStub.java).

### Application principale

![table](/INF111/images/TP3/hanoiSwing.png?width=40pc)

L'application principale va contenir la liste des tours et le panneau supérieur. L'application va aussi inclure un menu avec une option pour une nouvelle partie et la possibilité de quitter l'application.

* Type : JFrame
* Taille : 600 * 400
* Layout : BroderLayout, les tours seront dans le `CENTER` et le panneau supérieur sera dans le `PAGE_START`

### Pondération de correction
Consulter la [grille d'évaluation](/grilleevaluation.pdf) pour avoir plus d'informations.
