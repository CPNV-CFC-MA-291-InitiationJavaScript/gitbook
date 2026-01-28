# Feedback projet



## Introduction

Ce document est émis suite à une première évaluation de vos projets respectifs.

Il a pour intention de vous permettre de prioriser vos efforts pour cette dernière semaine de cours.

## Points positifs - à maintenir

Nombreuses sont les équipes à avoir très bien appliqué les pratiques suivantes:

* Séparation des couches logiques (layers) HTML, CSS et JS.
* Un effort particulier dans l'architecture (découpage en fonctions)
* Un résultat qui permet déjà d'avoir un retour d'expérience de la part d'un "end-users"

## TODO - Priorité 1 - Effort minimum

Voici la liste des points que vous pouvez corriger rapidement:

* [ ] Relire le cahier des charges et vérifier si vous répondez à tous les critères
* [ ] Finaliser les interfaces graphiques
  * [ ] Rappel : doit être compatible avec, a minima, un support de votre choix (mobile, tablette ou desktop)
  * [ ] Les trois zones de l'interface graphique doivent s'aligner et se positionner de manière cohérente entre elles.
* [ ] Commentaires
  * [ ] Retirer les commentaires qui n'apportent rien (//ceci est une boucle)
  * [ ] Convention de nommage pour les fichiers
    * [ ] Eviter les espaces
    * [ ] &#x20;Les majuscules utilisées de manières aléatoires
* [ ] Votre projet ne doit pas contenir de terme francophones
  * [ ] Excepté pour le readme si vous le désirez
  * [ ] Aucun nom de variable en français
  * [ ] Les commentaires (au sein du code) doivent également être rédigés en anglais
* [ ] Code "silencieux"
  * [ ] Retrier les variables inutiles
  * [ ] Retirer les fonctions qui ne sont pas exploitées par votre projet

## TODO - Priorité 2 - Effort moyen

* [ ] Le livrable doit être présent sur la branche develop
  * [ ] Vous êtes nombreux à n'avoir exploité que la branche main. Cette pratique doit être abandonnée aussi vite que possible.
  * [ ] Pour ceux qui ont créé des branches "feature" vous pouvez simplement les renommer "develop"

```bash
//créer la branche develop en se basant sur main

//1. vérifier que votre branche main est propre (git status)
git status (depuis la branche main)

//2a. créer la branche develop depuis main
git checkout -b develop

//3. vérifier que vous disposez bien de deux branches
git branch

//4. lors de la première livraison sur le dépôt, configurer l'upstream
git push --set-upstream origin develop
```

* [ ] Segment de code identique
  * [ ] L'environnement de développement va vous y aider
  * [ ] Il s'agit d'identifier du code similaire présent à différents endroits
  * [ ] De centraliser ce code identique dans une seule et même function
  * [ ] De supprimer le code identique et de le remplacer un appel à cette nouvelle fonction écrite.

```javascript
//exemple de code présentant de nombreuses lignes identiques   
case 'easy':
        num1 = Math.floor(Math.random() * 10);
        num2 = Math.floor(Math.random() * 10);
        operator = operators[Math.floor(Math.random() * 2)];
        break;
case 'medium':
        num1 = Math.floor(Math.random() * 50);
        num2 = Math.floor(Math.random() * 50);
        operator = operators[Math.floor(Math.random() * 4)];
        break;
case 'hard':
        num1 = Math.floor(Math.random() * 100);
        num2 = Math.floor(Math.random() * 100);
        operator = operators[Math.floor(Math.random() * 4)];
        break;
```

```javascript
//exemple de refactorisation

function generateFloat (factor) {
    return Math.floor(Math.random() * factor)
}

//simplification du case
case 'easy':
        num1 = generateFloat(10);
        num2 = generateFloat(10);
        operator = operators[generateFloat(2)];
        break;

//Note : ce n'est qu'un début de simplicfiation. Mais c'est ce niveau qui est attendu.

```

* [ ] Séparation de la couche métier et visuelle
  * [ ] Plusieurs méthodes js sont responsables de mettre à jour l'interface graphique en HTML/CSS. Jusqu'ici tout va bien.
  * [ ] Ces méthodes qui font le lien entre votre interface graphique et votre code métier ne doivent faire que cela.
    * [ ] Exemple : si vous réalisez des totaux, des mise à jour de valeur. Ceci est isolé dans une fonction. Puis une seconde fonction se charge de mettre à jour l'interface graphique.
*   [ ] La structure de votre projet

    * [ ] Le projet est contenu dans le projet git vs github. En ouvrant votre projet, on doit se retrouver directement dans le code et non pas en présence d'un répertoire qui lui-même contient le code.

    <figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

