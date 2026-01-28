# HTML5 et JS, qu'apporte-t-il ?

## Introduction

La vraie valeur ajoutée de JavaScript dans un site web est la personnalisation de l’expérience utilisateur. Alors que HTML et CSS seuls produisent des pages statiques à apparence fixe, JavaScript permet d’adapter le contenu et le comportement en fonction des interactions de l’utilisateur.&#x20;

Mieux encore, ce code peut évoluer au fil de la session, offrant une expérience dynamique, et, s’il est couplé à du stockage local ou à une API, il peut même conserver un état entre plusieurs visites.

## Les points fort du JS

### **HTML + CSS = rendu statique**

* Un site uniquement basé sur ces deux langages est **figé** : même contenu, même apparence, aucun comportement conditionnel.
* Les seules « variations » possibles sont liées aux _media queries_ CSS ou aux pseudo-classes (`:hover`, `:focus`…), mais ça reste limité et prédéfini.

### **JS = personnalisation de l’expérience**

* Avec JavaScript, l’interface peut réagir **en temps réel** aux actions de l’utilisateur.
* Exemple : affichage d’un message d’accueil personnalisé, filtres dynamiques, thèmes clairs/sombres choisis par l’utilisateur.

### **Évolution pendant la session**

* JavaScript permet de stocker des données en mémoire (variables, `sessionStorage`) et de modifier le comportement de la page **tant que la session dure**.
* Une fois la page rechargée, tout repart à zéro (sauf si on a utilisé `localStorage`, cookies ou une API côté serveur pour garder un état persistant).

