# Types et grammaire

## Les base du langage

* [ ] Sensible à la casse

{% code lineNumbers="true" %}
```javascript
let name = "Robert"
typeof Name;
```
{% endcode %}

{% hint style="info" %}
A la ligne 2, JavaScript mentionnera "undefined"
{% endhint %}

* [ ] Les "statements" est le terme utilisé pour signifier les instructions
  * [ ] Le ";" permet de spécifier la fin d'un statement, mais il est optionnel si vous n'avez qu'un seul statetement par ligne.

```javascript
let a; a=1+1; //exemple de cas obligeant l'utilisation du ";" 
```

* [ ] Les commentaires
  * [ ] sur une seule ligne nécessite "//"
  * [ ] sur plusieurs lignes nécessite "/\* pour l'ouverture et "\*/" pour la fermeture

{% code lineNumbers="true" %}
```javascript
// un commentaire sur une ligne

/* un commentaire plus
   long sur plusieurs lignes
 */

/* Par contre on ne peut pas /* imbriquer des commentaires */ SyntaxError */

```
{% endcode %}

* [ ] Les variables
  * [ ] pour les déclarer, on utilise un nom que l'on définit comme étant son identifiant.
  * [ ] règles de nommages:
    * [ ] débute par une lettre, un "\_" ou un symbole "$".
    * [ ] il est possible d'utiliser des chiffres, sauf en première position.
    * [ ] l'utilisation de minuscule et majuscule est permis également.

```javascript
var Nombre_touches
var temp99
const $credit
let _nom            //exemple d'identifiants autorisés 
```

<figure><img src="../../../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Comparatif des trois mot clés permettant de déclarer des variables, source : <a href="https://rixong.medium.com/var-let-and-const-28ab64ac2460">medium</a></p></figcaption></figure>
