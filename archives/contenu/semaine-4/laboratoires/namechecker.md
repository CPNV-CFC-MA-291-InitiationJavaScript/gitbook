# NameChecker

## Intentions pédagogiques

Entraîner de manière partique la création et l'utilisation d'exceptions personnalisées.

## Objectifs opérationnels

* Etudier l'exemple "AgeChecker"
* Etudier la solution proposée (à l'aide d'un enchaînement de if/else)
* Fork ce dépôt

{% embed url="https://github.com/CPNV-InitiationJavaScript/ExceptionHandling" %}

* En vous inspirant de AgeChecker, adapter le code livré "EmailChecker"
* Livrer le code sur votre dépôt pour la review réalisée en classe

### Exemple AgeChecker

Déterminer si une personne est majeure ou mineur en fonction de son âge.

### Solution proposée

{% code fullWidth="false" %}
```javascript
// Définition d'une exception personnalisée
class AgeValidationError extends Error {
    constructor(message) {
        super(message);  // Appelle le constructeur de la classe parent (Error)
        this.name = "AgeValidationError";  // Nom de l'erreur
    }
}

// Fonction de validation de l'âge
function validateAge(age) {
    if (age < 18) {
        throw new AgeValidationError("L'utilisateur doit être majeur (18 ans et plus).");
    }
    return "Validation réussie. L'utilisateur est majeur.";
}

// Utilisation de la fonction avec gestion des exceptions
try {
    let result;
    console.log("Test avec un majeur");
    result = validateAge(18);
    console.log(result);

    console.log("Test avec un mineur");
    result = validateAge(16);  // Change l'âge pour tester différents scénarios
    console.log(result);

} catch (error) {
    if (error instanceof AgeValidationError) {
        console.error("Erreur de validation d'âge : " + error.message);
    } else {
        console.error("Erreur inattendue : " + error.message);
    }
}
```
{% endcode %}
