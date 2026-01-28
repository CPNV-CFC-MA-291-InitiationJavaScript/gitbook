# Standard ECMAScript

## JavScript et la spécification ECMA Script

JavaScript est standardisé par [Ecma International](https://www.ecma-international.org/) — une association européenne de standardisation des systèmes d'information et de communication (ECMA étant historiquement un acronyme pour _European Computer Manufacturers Association_) qui délivre un langage de programmation standardisé, international appelé ECMAScript. Ce langage se comporte de la même façon pour toutes les applications qui supportent ce standard. Les entreprises peuvent utiliser ce langage standard afin de développer leur implémentation de JavaScript. Le standard ECMAScript est documenté avec la spécification ECMA-262.

{% hint style="info" %}
TODO : Vérifier bien que dans votre IDE, la norme soit bien la 6.
{% endhint %}

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption><p>Ecran WebStorm validant l'activation d'ECMA6 et suivant</p></figcaption></figure>

La spécification ECMAScript est un ensemble de conditions à respecter pour implémenter ECMAScript : cela est utile lorsqu'on souhaite implémenter des fonctionnalités standard du langage au sein d'une implémentation ou d'un moteur ECMAScript (tel que SpiderMonkey pour Firefox, ou V8 pour Chrome).

La spécification ECMAScript n'a pas pour but d'aider les développeurs à écrire des scripts. La documentation JavaScript permet d'obtenir des informations pour écrire des scripts JavaScript.

La spécification ECMAScript utilise parfois une terminologie et une syntaxe qui peuvent sembler étranges aux yeux d'un développeur JavaScript. Bien que la description du langage diffère entre ECMAScript et la documentation JavaScript, le langage lui-même reste le même. JavaScript supporte l'ensemble des fonctionnalités mises en avant dans la spécification ECMAScript.

La documentation JavaScript décrit les aspects du langage qui pourront être utilisés par les développeurs JavaScript.

## Exemples

### Let

"The **let** variables are mutable i.e. their values can be changed. It works similarly to the var keyword with some key differences like scoping which makes it a better option when compared to var.

**Example:** This example will illustrate how to declare a variable using the let keyword."

```javascript
// Const 
const name = 'Mukul';
console.log(name); 
// Will print 'Mukul' to the console.

// Trying to reassign a const variable
name = 'Rahul';
console.log(name); 
// Will give TypeError.

// Trying to declare const variable first
// and then initialize in another line
const org_name;
org_name = "GeeksforGeeks";
console.log(org_name);
// Throws a syntax error: missing initializer in const declaration
```

Source : [geeksforgeeks.org](https://www.geeksforgeeks.org/introduction-to-es6/#const)



{% hint style="info" %}
TODO : en lisant [ce document](https://www.geeksforgeeks.org/javascript-let/), tester et valider à l'aide de votre IDE la notion de "scope"
{% endhint %}
