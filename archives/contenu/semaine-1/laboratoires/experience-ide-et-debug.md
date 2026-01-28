# Expérience IDE et Debug

## Objectifs du lab

* [ ] Installation de l'environnement de développement
* [ ] Créer un premier projet
* [ ] Exécuter un script
* [ ] Se familiariser avec le debugger

## Installation de l'IDE

* [Récupérer l'installeur](https://www.jetbrains.com/webstorm/download/#section=windows)
* [S'inscrire chez JetBrains (même compte que pour pycharm)](https://www.jetbrains.com/shop/eform/students)
* S'authentifier dans l'IDE pour récupérer la licence

## Créer un premier projet

* Lancer WebStorm
* Ajouter la dépendence nodejs

{% embed url="https://nodejs.org/en/download/prebuilt-installer" %}

* Créer un nouveau projet (vide)

<figure><img src="../../../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Ne positionner pas vos projets ni sur un lecteur réseau, ni dans un répertoire synchroniser avec oneDrive (ou autre) ni à la racine de C:\
\
Idéalement, au sein de C:\Users\\\<MyName>\\\<MyDevs>\\\<MyProject>
{% endhint %}

* Créer un nouveau fichier et insérer ce contenu

```javascript
/*
Author : Nicolas Glassey
Title  : some simple javascript samples
 */

const message = "La somme de "
let a = 15
let b = 20
let sum = a + b
let messageToDisplay = message + a + " et " + b + " = " + sum
console.log(messageToDisplay)
```

* Exécuter le script et observer le résultat dans la console

<figure><img src="../../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

* Placer un point d'arrêt

<figure><img src="../../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

* Relancer en mode debug

<figure><img src="../../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

* Observer le contenu des variables

<figure><img src="../../../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
