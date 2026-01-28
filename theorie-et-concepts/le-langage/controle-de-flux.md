# Contrôle de flux

Les **instructions de contrôle de flux** en JavaScript permettent de modifier l'exécution d'une boucle ou d'une fonction :

* **`break`** : Interrompt une boucle ou un `switch`.

```javascript
for (let i = 0; i < 10; i++) {
  if (i === 5) break;  // Interrompt la boucle à 5
  console.log(i);
}
```

* **`continue`** : Saute à l'itération suivante d'une boucle.

```javascript
for (let i = 0; i < 10; i++) {
  if (i === 5) continue;  // Saute l'affichage de 5
  console.log(i);
}
```

* **`return`** : Interrompt une fonction et retourne une valeur.

```javascript
function checkNumber(num) {
  if (num < 0) return "Négatif";  // Arrête la fonction si num est négatif
  return "Positif";
}
```



