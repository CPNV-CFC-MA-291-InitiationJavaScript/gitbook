# Instruction de contrôle

## Introduction

Le contrôle de flux en JavaScript fait référence à <mark style="color:orange;">la manière dont l'exécution du code est dirigée</mark> en fonction de certaines conditions. Il permet au programme de prendre des décisions, répéter des actions ou gérer des exceptions.&#x20;

## Instructions conditionnelles

**`if...else`** : Utilisé pour exécuter du code en fonction d'une condition. Si la condition est vraie, un bloc de code est exécuté, sinon un autre bloc (facultatif) est exécuté.

```javascript
if (condition) {
  // code si condition est vraie
} else {
  // code si condition est fausse
}
```

**`else if`** : Permet d'ajouter plusieurs conditions à tester avant d'atteindre le bloc `else` final.

```javascript
if (condition1) {
  // code si condition1 est vraie
} else if (condition2) {
  // code si condition2 est vraie
} else {
  // code si aucune des conditions n'est vraie
}
```

**`switch`** : Utile lorsque vous avez plusieurs valeurs possibles à tester. Il compare une expression à différents cas.

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

## Boucle (répétitions)

**`for`** : Boucle classique pour répéter un bloc de code un nombre spécifique de fois.

```javascript
for (let i = 0; i < 10; i++) {
  // code exécuté 10 fois
}
```

**`while`** : Répète le bloc tant qu'une condition est vraie.

```javascript
while (condition) {
  // code tant que condition est vraie
}
```

**`do...while`** : Similaire à `while`, mais le bloc est exécuté au moins une fois avant de vérifier la condition.

```javascript
do {
  // code exécuté au moins une fois
} while (condition);
```

**`for...of`** : Itère sur les éléments d'une collection (comme un tableau).

```javascript
for (const element of tableau) {
  // code pour chaque élément
}
```

**`for...in`** : Itère sur les propriétés énumérables d'un objet.

```javascript
for (const key in objet) {
  // code pour chaque clé de l'objet
}
```

