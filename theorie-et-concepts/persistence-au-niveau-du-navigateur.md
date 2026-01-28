# Persistence au niveau du navigateur



## Introduction

Lorsque l'on recharge la page web, on retrouvera la situation initiale si notre javascript ne tourne qu'en mémoire vive.

JavaScript permet justement de contourner ça en **persistant des données** (localStorage, IndexedDB, cookies) ou en **reparlant au serveur** via des API → ce qui donne l’impression que l’expérience « continue » entre les sessions.

Conclusion:

* **Sans JS** : le site est une **vitrine statique**.
* **Avec JS** : le site devient une **application vivante**, qui s’adapte **pendant la session** et qui peut même s’inscrire dans une logique de persistance si besoin.

## **La notion de session**

La _session_ désigne la période pendant laquelle un utilisateur interagit avec une application entre deux rechargements ou connexions.

{% hint style="warning" %}
**Sans stockage particulier**, les variables JS n’existent que tant que la page est ouverte
{% endhint %}

```javascript
let compteur = 0;
compteur++;
console.log(compteur); // 1
// un rechargement de la page réinitialisera le compteur
```

Pour **mémoriser** des données au-delà de simples variables temporaires, on utilise des API de stockage comme `sessionStorage` ou `localStorage`.

## **SessionStorage**

* Stocke des données **le temps de la session** → elles disparaissent quand tu fermes l’onglet ou le navigateur.
* Utilisation typique : garder un état temporaire pendant que l’utilisateur navigue sur le site.

```javascript
// Sauvegarder une donnée
sessionStorage.setItem("theme", "dark");

// Lire la donnée
console.log(sessionStorage.getItem("theme")); // "dark"

// Supprimer une donnée
sessionStorage.removeItem("theme");

// Vider complètement
sessionStorage.clear();
```

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption><p>Observation d'une variable de session sur Firefox<br>(Sur Chrome il supportera l'appelle même sur une page blanche, mais pas Firefox)</p></figcaption></figure>

## **LocalStorage**

* Très similaire à `sessionStorage`, mais <mark style="color:orange;">**persiste même après avoir fermé le navigateur**</mark>.
* Les données restent disponibles tant qu’elles ne sont pas supprimées (manuellement ou par code).

```javascript
// Sauvegarder une donnée persistante
localStorage.setItem("langue", "fr");

// Lire la donnée
console.log(localStorage.getItem("langue")); // "fr"

// Même après avoir fermé et rouvert le navigateur, ça reste
```

## **Synthèse**

| Stockage           | Durée de vie                     | Portée                                | Exemple d’usage                       |
| ------------------ | -------------------------------- | ------------------------------------- | ------------------------------------- |
| **Variable JS**    | Tant que la page est chargée     | Mémoire de la page                    | Compteur temporaire                   |
| **sessionStorage** | Tant que l’onglet est ouvert     | Spécifique à l’onglet                 | Panier pendant la navigation          |
| **localStorage**   | Persistant (jusqu’à suppression) | Partagé entre onglets du même domaine | Sauvegarde de préférences utilisateur |
