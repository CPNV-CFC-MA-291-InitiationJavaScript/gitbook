# Back-end / Front-end - cas d'études

## Objectif

Analyser un petit projet de "e-commerce" et mettre évidence ce qui va être de la responsabilité du front-end et du back-end.

## Cas des charges simplifié

Votre client désire réaliser le développement d'une application de réservation de pizza. Il s'agit d'un "food truck" qui actuellement gère les réservations, au jour le jour, via son téléphone mobile.

Les clients  peuvent réserver via un message what's app hors des heures d'ouvertures du "food truck". Lorsque le "food truck" est installé sur son emplacement du jour, les clients appellent pour réserver. Une toute petite partie des clients commandes directement sur place mais ce cas peut-être ignorer.

<figure><img src="../../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### Améliorations attendues grâce à l'application

### Panier de réservation

L'application doit pouvoir remplacer les messages what's app par des demandes de réservation en ligne.  Le comportement doit être similaire à un panier de e-commerce,&#x20;

<figure><img src="../../../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Exemple de panier remplaçant les actuels messages what's app</p></figcaption></figure>

Le processus s'arrête dès que la réservation est confirmée, par l'envoi d'un email au client. On ne gère pas la notion de payement.

#### Gestion des heures de livraisons souhaitées

Le système doit être capable de gérer les "collisions" de réservation, autrement dit éviter que plusieurs personnnes ne commandent pour la même heure.

La capacité de production du "food truck" est de 2 pizzas toutes les 3 minutes.

Lorsque le client clique sur "Réserver" le système doit lui proposer les prochaines heures de livraison possibles, en prenant en compte le nombre de pizzas demandées pour cette nouvelle réservation ainsi que les réservations des autres clients.

TODO

Identifier les différentes fonctionnalités

Classez-les "front-end" ou "back-end"

