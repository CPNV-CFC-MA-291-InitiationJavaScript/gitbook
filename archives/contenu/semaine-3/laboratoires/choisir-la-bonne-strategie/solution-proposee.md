# Solution proposée

## Solution à l'aide d'un switch case

```javascript
function getDaySwitch(day) {
    switch (day) {
        case 1:
            return "Lundi";
        case 2:
            return "Mardi";
        case 3:
            return "Mercredi";
        case 4:
            return "Jeudi";
        case 5:
            return "Vendredi";
        case 6:
            return "Samedi";
        case 7:
            return "Dimanche";
        default:
            return "Numéro de jour invalide";
    }
}

console.log(getDaySwitch(3));  // "Mercredi"
```

## Solution à l'aide d'une boucle (sur un tableau)

```javascript

function getDayFor(day) {
    const days = ["Lundi", "Mardi", "Mercredi", "Jeudi", "Vendredi", "Samedi", "Dimanche"];

    for (let i = 0; i < days.length; i ++) {
        if (day === i + 1) {
            return days[i];
        }
    }
    return "Numéro de jour invalide";
}

console.log(getDayFor(3));  // "Mercredi"

```
