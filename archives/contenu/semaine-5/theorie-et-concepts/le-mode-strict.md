# Le mode strict

## Introduction

Le mode strict de [ECMAScript 6](https://www.ecma-international.org/publications/standards/Ecma-262.htm) <mark style="color:orange;">permet de choisir une variante restrictive de JavaScript</mark>. Le mode strict n'est pas seulement un sous-ensemble de JavaScript : il possède _intentionnellement_ des sémantiques différentes du code normal.&#x20;

<mark style="color:orange;">Les navigateurs ne supportant pas le mode strict</mark> exécuteront le code d'une façon légèrement différente de ceux le supportant, il ne faut donc pas compter sur le mode strict pour éviter des tests sur les navigateurs qui ne le supportent pas.&#x20;

<mark style="color:orange;">Les codes en mode strict et en mode non-strict peuvent coexister, ce qui permet de réécrire les scripts en mode strict de façon incrémentale.</mark>

Le mode strict apporte quelques changements à la sémantique « normale » de JavaScript:

1. Le mode strict élimine quelques <mark style="color:orange;">erreurs silencieuses</mark> de JavaScript en les changeant <mark style="color:orange;">en erreurs</mark> explicites (une exception sera levée).
2. Le mode strict corrige les erreurs qui font qu'autrement il est difficile pour les moteurs JavaScript d'effectuer des optimisations. <mark style="color:orange;">Le code sera donc exécuté plus rapidement en mode strict</mark>, sans changer une seule ligne si cela n'est pas nécessaire.
3. Le mode strict <mark style="color:orange;">interdit les mot-clés</mark> susceptibles d'être définis dans les futures versions de ECMAScript.

## Le mode strict pour les scripts

Pour invoquer le mode strict pour un script entier, on ajoutera l'instruction exacte `"use strict";` (ou `'use strict';`) avant toutes les autres instructions.

```javascript
// Script entier en mode strict
"use strict";
var v = "Allo ! Je suis en mode strict !";
```

## Différences du mode strict <a href="#differences_du_mode_strict" id="differences_du_mode_strict"></a>

Le mode strict modifie <mark style="color:orange;">à la fois la syntaxe et le comportement à l'exécution</mark>. Les changements se déclinent généralement en trois catégories:&#x20;

* ceux qui convertissent les fautes en erreurs (comme des erreurs de syntaxe ou les erreurs d'exécution),&#x20;
* ceux qui simplifient comment une variable pour un nom donné est traitée, simplifiant [`eval()`](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/eval) et [`arguments`](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Functions/arguments) et,
* ceux qui permettent d'écrire plus simplement du code JavaScript pérenne qui anticipe les évolutions futures d'ECMAScript.

### Convertir les fautes en erreurs <a href="#convertir_les_fautes_en_erreurs" id="convertir_les_fautes_en_erreurs"></a>

Premièrement, en mode strict, il est impossible de créer accidentellement des variables globales. En mode normal, ne pas déclarer une variable lors d'une affectation (oublier l'instruction [`var`](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Statements/var)) crée une nouvelle propriété sur l'objet global et le code continue de fonctionner (même si ça peut être une source de problèmes par la suite). Les affectations qui pourraient accidentellement créer des variables globales lèveront une erreur en mode strict:

```javascript
"use strict";
variableMalDéclarée = 17; // lève une ReferenceError
```
