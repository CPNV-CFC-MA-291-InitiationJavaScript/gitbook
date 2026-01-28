# Instruction de contrôle

## Introduction

Le contrôle de flux en JavaScript fait référence à <mark style="color:orange;">la manière dont l'exécution du code est dirigée</mark> en fonction de certaines conditions. Il permet au programme de prendre des décisions, répéter des actions ou gérer des exceptions.&#x20;

## Instructions conditionnelles

**`if...else`** : Utilisé pour exécuter du code en fonction d'une condition. Si la condition est vraie, un bloc de code est exécuté, sinon un autre bloc (facultatif) est exécuté.

{% code lineNumbers="true" %}
```javascript
if (condition) {
  // code si condition est vraie
} else {
  // code si condition est fausse
}
```
{% endcode %}

**`else if`** : Permet d'ajouter plusieurs conditions à tester avant d'atteindre le bloc `else` final.

{% code lineNumbers="true" %}
```javascript
if (condition1) {
  // code si condition1 est vraie
} else if (condition2) {
  // code si condition2 est vraie
} else {
  // code si aucune des conditions n'est vraie
}
```
{% endcode %}

**`switch`** : Utile lorsque vous avez plusieurs valeurs possibles à tester. Il compare une expression à différents cas.

{% code lineNumbers="true" %}
```javascript
switch (expression) {
  case valeur1:
    // code si expression === valeur1
    break;
  case valeur2:
    // code si expression === valeur2
    break;
  default:
    // code si aucune valeur ne correspond
}
```
{% endcode %}

## Boucle (répétitions)

**`for`** : Boucle classique pour répéter un bloc de code un nombre spécifique de fois.

{% code lineNumbers="true" %}
```javascript
for (let i = 0; i < 10; i++) {
  // code exécuté 10 fois
}
```
{% endcode %}

**`while`** : Répète le bloc tant qu'une condition est vraie.

{% code lineNumbers="true" %}
```javascript
while (condition) {
  // code tant que condition est vraie
}
```
{% endcode %}

**`do...while`** : Similaire à `while`, mais le bloc est exécuté au moins une fois avant de vérifier la condition.

{% code lineNumbers="true" %}
```javascript
do {
  // code exécuté au moins une fois
} while (condition);
```
{% endcode %}

**`for...of`** : Itère sur les éléments d'une collection (comme un tableau).

{% code lineNumbers="true" %}
```javascript
for (const element of tableau) {
  // code pour chaque élément
}
```
{% endcode %}

**`for...in`** : Itère sur les propriétés énumérables d'un objet.

{% code lineNumbers="true" %}
```javascript
for (const key in objet) {
  // code pour chaque clé de l'objet
}
```
{% endcode %}

