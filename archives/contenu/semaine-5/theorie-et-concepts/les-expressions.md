# Les expressions

Source: [Mozilla Foundations](https://developer.mozilla.org/fr/docs/Web/JavaScript/Guide/Expressions_and_operators)

## Introduction

Dans ce chapitre, nous décrirons les expressions et opérateurs en JavaScript, qui permettent notamment:

* l'affectation,
* la comparaison,
* les opérations arithmétiques, binaires, logiques,&#x20;
* la manipulation de chaîne de caractères, etc.

### Les types d'expressions

<mark style="color:orange;">Une</mark> <mark style="color:orange;"></mark>_<mark style="color:orange;">expression</mark>_ <mark style="color:orange;"></mark><mark style="color:orange;">peut être vue comme une unité de code valide qui est résolue en une valeur</mark>. Il existe deux types d'expressions:&#x20;

* celles qui ont des effets de bord (par exemple l'affectation d'une valeur),
* celles qui sont purement évaluées.

```
x = 3 + 4
```

```
3 + 4 // fait partie de la seconde catégorie, évaluée sans effet de bord
x = 7 // fait partie de la première catégorie, avec l'affectaction d'une valeur à x
```

#### Quelques autres exemples

| Nom                                                                                                                                    | Opérateur  | Signification |
| -------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ------------- |
| [Affectation](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Operators/Assignment)                                     | `x = f()`  | `x = f()`     |
| [Affectation après addition](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Operators/Addition_assignment)             | `x += f()` | `x = x + f()` |
| [Affectation après soustraction](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Operators/Subtraction_assignment)      | `x -= f()` | `x = x - f()` |
| [Affectation après multiplication](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Operators/Multiplication_assignment) | `x *= f()` | `x = x * f()` |
| [Affectation après division](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Operators/Division_assignment)             | `x /= f()` | `x = x / f()` |
| [Affectation du reste](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Operators/Remainder_assignment)                  | `x %= f()` | `x = x % f()` |

## Affectations aux propriétés

{% hint style="info" %}
Une propriété est une méthode permettant d'accéder en écriture ou/et en l'écrire à l'attribut d'un objet.
{% endhint %}

```javascript
const obj = {};

obj.x = 3;
console.log(obj.x); // Affiche 3.
console.log(obj); // Affiche { x: 3 }.

const key = "y";
obj[key] = 5;
console.log(obj[key]); // Affiche 5.
console.log(obj); // Affiche { x: 3, y: 5 }.
```

