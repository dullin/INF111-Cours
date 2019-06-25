+++
title = "Héritage"
menuTitle = "Héritage"
draft = false
weight = 5030
+++

L'héritage est orienté-objet est la relation entre une classe d'une classe plus générique (la `superclasse`) et une classe plus spécialisée (la `sous-classe`).

Pour avoir une classe spécialisée, on utilise le mot clé `extend` à la création de la classe.

```java
public class MaClasse {
    // Stuff
}

public class MaClasseSpeciale extends MaClasse {
    // More stuff
    // Hérite les méthodes de MaClasse
}
```

Il faut faire attention, les variables d'instances privées de la classe générale ne sont pas accessibles par la classe spécialisée.