# Choisir la bonne stratégie

## Intentions pédagogiques

Entraîner de manière partique les différentes formes d'instructions conditionnelles vues en théorie et pouvoir comparer leur pertinence en fonction d'un contexte donné.

## Objects opérationnels

* [ ] Etudier la situation décrite
* [ ] Etudier la solution proposée (à l'aide d'un enchaînement de if/else)
* [ ] Fork ce dépôt

{% embed url="https://github.com/CPNV-InitiationJavaScript/ControlFlow" %}

* [ ] Refactoriser la solution proposée en utilisant un switch case
* [ ] Refactoriser la solution proposée en utilisant une boucle
* [ ] Livrer les trois solutions dans des fichiers séparés:
  * [ ] weeklyDayIfElse.js
  * [ ] weeklyDaySwitchCase.js
  * [ ] weeklyDayLoop.js

### Situation à solutionner

Déterminer le jour de la semaine en fonction d'un numéro (1 à 7).

### Solution "if/else"

```javascript
function getDayIfElse(day) {
  if (day === 1) {
    return "Lundi";
  } else if (day === 2) {
    return "Mardi";
  } else if (day === 3) {
    return "Mercredi";
  } else if (day === 4) {
    return "Jeudi";
  } else if (day === 5) {
    return "Vendredi";
  } else if (day === 6) {
    return "Samedi";
  } else if (day === 7) {
    return "Dimanche";
  } else {
    return "Numéro de jour invalide";
  }
}

console.log(getDayIfElse(3));  // "Mercredi"
```

