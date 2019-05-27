+++
title = "Affichage"
menuTitle = "Affichage"
draft = false
weight = 70
+++

L'affichage de nos programmes se font dans la fenêtre de commande avec les méthodes d'affichages fournies par Java.

### Méthode `println`
La méthode `println` permet d'afficher une chaine de caractères suivit d'un saut de ligne.

```java
// La méthode doit être invoqué de l'objet globale System et de sa propriété out.
// Nous verrons en détails plus tards les principes d'objets et de propriétés.
System.out.println("Bonjour la classe!");
```

### Interprétation de l'expression dans l'affichage

Les méthodes d'affichage sont capable de recevoir plusieurs types de données et les convertirs en chaine de caractères pour l'affichage.
L'opérateur `+` est utilisé pour faire la concaténation de différents éléments de l'affichage.

```java
int x = 5;
String nom = "Bob";
System.out.println("Le nom est : " + nom + ". Et x vaut : " + x + ".");
```

### Formatage de l'affichage avec `printf`

Pour avoir plus de contrôle sur les paramètres d'affichage, `printf` nous donne accès à des options additionnelles pour l'affichage.
`printf` utilise des opérateurs de formatage dans un chaine de caractères pour ensuite remplir les opérateurs utilisé.

```java
double x = 4.54242234;
// Limite le nombre de décimal à afficher
System.out.printf("Le nombre : %.2f", x);
```

### Références

https://docs.oracle.com/javase/tutorial/java/data/numberformat.html