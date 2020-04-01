# McommerceActivites

Je suis sensé faire:

Partie 1 : création d'un nouveau Microservice

1- Créez un nouveau Microservice et nommez-le  microservice-expedition. Ce Microservice doit :
intégrer les starters web, Actuator, JPA et H2,
avoir un nom déclaré,
écouter le port 9006.
2- Créez une classe Expedition dans un package appelé model avec comme attributs :  id ,  idCommande  et  etat .
3- Créez une méthode qui répond aux requêtes de type POST et qui permet d’ajouter une nouvelle expédition à la base de données.
Par exemple, si vous exécutez une requête POST avec le JSON suivant :

{
   "id": 2,
   "idCommande": 3,
   "etat": 1
 }

4- Créez une méthode qui permet de récupérer une expédition par son id.
5- Créez une méthode qui permet de mettre à jour une expédition.
Partie 2 : interface de visualisation
Dans ClientUI, créez une page qui affiche l’état de la commande.
Les états possibles sont les suivants : 
0 : En préparation
1 : Expédiée
2 : Livrée
Pour cela :
1) Ajoutez Ribbon à microservice-expedition
2) Pour faire appel à microservice-expedition vous devez utiliser Feign
Le rôle de Feign est :
d'utiliser Ribbon pour aller chercher l’URL,
d'envoyer les requêtes en passant par l’API Gateway ZUUL.
3) Ajoutez Eureka à microservice-expedition.
4) Faites les modifications nécessaires afin que les requêtes générées par Feign via le proxy d’expédition passent par ZUUL.
 

