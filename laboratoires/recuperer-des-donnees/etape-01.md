# Etape 01

## Intention

Dans ce laboratoire nous allons partir d'un site existant et analyser son comportement d'un point de vue de la gestion des données.

## Objectif

Il s'agira de réussir à obtenir un résultat similaire (en terme d'affichage), à la différence prêt que les 6 articles présentés ci-dessous devront être récupéré et affiché grâce à un script écrit en JavaScript.

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

### Tâche 001 - Récupérer le code existant

Créer un nouveau projet sous Webstorm et intégré ces deux fichiers:

{% file src="../../.gitbook/assets/source.zip" %}

Voici la structure à respecter:

```

└───data
        products.json
└───src
    │   index.html
    │
    └───assets
        └───css
                main.css
        └───imgs
                prod1.png
                prod2.png
                ...
        └───js
                fetchProduct.js
```

### Tâche 002 - Modéliser les articles

Les six articles devront provenir d'un fichier JSON que le script utilisera pour construire l'affichage des articles.

* [ ] Identifier les attributs: le fichier json devra contenir un liste de produit décrivant chacun des attributs.
* [ ] Images : le Json ne contiendra que les chemins vers les fichiers.

### Tâche 003 - Constuire le code HTML

* [ ] Construire (extraire) le code HTML qui "recevra" les données.

### Tâche 004 - Ecrire le script de génération d'articles

* [ ] Réaliser un script qui récupérera (fetch) les données présentes dans le json
* [ ] Produira le code HTML intégrant les valeurs.

### Tâche 005 - Afficher le résultat

La page index.html est responsable:

* [ ] de lancer le script
* [ ] d'intégrer le contenu produit et de l'afficher.



### Séquence à réaliser

<figure><img src="../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>





