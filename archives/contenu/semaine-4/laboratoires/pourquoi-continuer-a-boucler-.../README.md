# Pourquoi continuer à boucler ...

## Intentions pédagogiques

Dans ce laboratoire nous entraînons l'utilisation des mécanismes de contrôle de flux de JavaScript (control flow statements).

## Objectifs opérationnels

En partant d'un code livré, il vous sera demandé les tâches suivantes:

* [ ] forker le dépôt suivant:

{% embed url="https://github.com/CPNV-InitiationJavaScript/controlFlowStatements.git" %}

### Tâche 01 - Break

* [ ] étudier le code "break.js" et l'exécuter sur votre environnement
  * [ ] ajouter le code nécessaire pour identifier le premier nombre qui est supérieur à 50.
  * [ ] faites en sorte, <mark style="color:orange;">à l'aide d'un</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`break`</mark> que la boucle s'arrête dès que la condition est réalisée
  * [ ] observer le gain d'opération réalisées
  * [ ] présenter les résultats dans un tableau excel (pour 10 utilisations).
* [ ] identifier les endroits du code qui pourra mettre en oeuvre un contrôleur de flux,
* [ ] mettre en place un mécanisme qui va compter le nombre d'opérations que votre amélioration a permis d'éviter à votre machine.
* [ ] livrer votre solution sur votre dépôt
  * [ ] le message du commit est : "feat: break on time"

### Tâche 02 - Continue

* [ ] étudier le code "continue.js" et l'exécuter sur votre environnement (il s'agit du même code de départ que pour l'exercice précédent)
  * [ ] ajouter le code nécessaire pour réaliser une somme des éléments présents dans la liste.
  * [ ] modifier le code pour faire en sorte que seuls les "plus grands" nombres soient pris en compte, ceci à l'<mark style="color:orange;">aide d'un</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`continue`</mark>:
    * [ ] On lance la boucle.&#x20;
      * [ ] Le nombre le plus grand est pour l'instant égal à 0.
      * [ ] La somme est également égale à 0.
    * [ ] On prend le prochain élément, il est vaut (par exemple) 10.
      * [ ] Le nombre le plus grand passe à 10.
      * [ ] La somme passe à 10.
    * [ ] On continue d'analyser le tableau mais on ne prendra en compte que les valeurs qui sont supérieures à 10.
      * [ ] On identifie 8, on prend l'élément suivant.
      * [ ] On identifie 11:
        * [ ] Le nombre le plus grand passe à 11.
        * [ ] La somme passe à 21.
        * [ ] .... ainsi de suite
  * [ ] livrer votre solution sur votre dépôt
    * [ ] le message du commit est : "feat: continue better"

### Tâche 03 - Return

* [ ] étudier le code "return.js" et l'exécuter sur votre environnement (il s'agit du même code de départ que pour l'exercice précédent).
* [ ] ajouter le code nécessaire pour réaliser une soustraction en partant de 100 et déduisant la valeur de chaque élément de la liste. Le programme s'arrêt dès que vous avez traité toute la liste. La somme finale peu être négative.
* [ ] modifier le code pour faire en sorte que seuls les nombres paires soient soustrait (avec le mécanisme de votre choix).
* [ ] modifier encore le code pour stopper le code et retourner, <mark style="color:orange;">à l'aide d'un</mark> <mark style="color:orange;"></mark><mark style="color:orange;">`return`</mark> la somme restante dès qu'un des critères est satisfait:
  * [ ] vous avez traité plus de la moitié de la liste,
  * [ ] vous rencontrez une deuxième fois le même nombre à soustraire (vous vous arrêtez avant de le soustraire à nouveau),
  * [ ] vous avez atteint la somme résiduelle de 50 (valeur exacte, sinon on continue).
    * [ ] retourner le montant résiduel et la raison de l'arrêt de la boucle.
* [ ] livrer votre solution sur votre dépôt.
  * [ ] le message du commit est : "feat: return asap"

