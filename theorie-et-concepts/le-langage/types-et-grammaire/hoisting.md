# Hoisting

Source : [MDN](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)

## Qu’est-ce que le _hoisting_ en JavaScript ?

* _MDN définit le hoisting comme :_\
  **le processus par lequel l’interpréteur semble déplacer la déclaration des fonctions, variables, classes ou imports en haut de leur portée (scope) avant l’exécution du code.**
* Ce terme n’existe pas dans le langage normatif ECMAScript, bien que la spécification mentionne les _HoistableDeclaration_ pour les déclarations de fonctions `function`, `async function` et similaires. En pratique, on parle aussi couramment de hoisting pour les déclarations `var`, `let`, `const`, classes et imports, mais chacun se comporte différemment.

## Comportements selon le type de déclaration

**1. Fonctions (declaration)**

* Les déclarations de fonctions (e.g. `function foo() {}`) sont **entièrement hoistées** — nom et corps de la fonction sont disponibles dès le début du scope. Tu peux appeler la fonction avant même de l’avoir déclarée [developer.mozilla.org+1](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting?utm_source=chatgpt.com).

**2. Variables avec `var`**

* Le mot-clé `var` est hoisté : seule la **déclaration** est déplacée en haut, **mais pas l'initialisation**. Avant l’exécution, la variable existe avec la valeur `undefined`. Exemple typique:

```javascript
console.log(x); // undefined
var x = 5;
```

**3. Variables avec `let`, `const` et classes**

* Ces déclarations sont **également hoistées**, mais se trouvent dans une **« zone morte temporelle »** (Temporal Dead Zone) entre le début du scope et la ligne de déclaration. Tenter d’y accéder avant leur déclaration entraîne une **ReferenceError.**

**4. Imports**

* Les déclarations `import` sont aussi hoistées. Autrement dit, les identifiants importés sont disponibles dans tout le module, et leurs effets (comme les modules exécutés pour leurs effets secondaires) se produisent **avant le reste du code** du module.
