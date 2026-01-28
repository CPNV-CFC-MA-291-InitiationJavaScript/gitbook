# Introduction Git

## Comment forker un dépôt ?

* Se connecter sur le dépôt de l'enseignant
* Utiliser l'interface web pour générer un fork

<figure><img src="../../../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

* Cloner son dépôt (et non le dépôt de l'enseignant

```
git clone <monUrl>
```

<figure><img src="../../../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

## Séquence de base à maîtriser

* Réaliser des modifications sur le projet et identifier les changements

```
git status
```

* Préparer un "stage" pour un futur commit

```
git add .
```

* Créer une nouvelle version de votre code en "committant"

```
git commit -m "<prefix:...>"
```



{% hint style="info" %}
Préfixes à connaître:\
\
feat: -> contenu en lien avec une "feature"

test: -> contenu en lien avec des tests

fix: -> contenu qui corrige une erreur

chore:-> contenu qui n'impact pas le code (mise à jour gitignore, readme...)

refactor:-> contenu qui a permi d'améliorer le code (sans ajout de fonctionnalité)
{% endhint %}

* Livrer le contenu sur votre dépôt

```
git push
```

