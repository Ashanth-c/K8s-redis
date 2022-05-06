# Explication

## deployment_redis_ac.yaml

Ce fichier lance le pod de redis sur un conteneur avec comme port de connexion 6379

## deployment_serveur_ashanth.yaml

Ce fichier lance le pod d'un serveur node-redis privé sur un conteneur avec comme port de connexion 4000.
On indique aussi en parametre d'environnement son port de connexion ainsi que l'URL de redis afin de pouvoir s'y connecter.
Le nombre de pods créé au deploiement est de 4

## service_redis-ashanth.yaml

Ce fichier service permet d'indiquer les ports de connexion du pod créé avec le deployment_redis_ac.yaml

## service_serveur-ashanth.yaml

Ce fichier service permet d'indiquer les ports de connexion du pod créé avec le deployment_redis_ac.yaml

## Nom des pods

redis : redis-ac
serveur redis : ac-redis-serveur

# Bonus

## Etape 1 Creer un Dockerfile pour l'application react

Utiliser la commande docker build -t reactapp ./bonus/redis-react 

## Etape 2 Creer un fichier deployment.yaml

ici notre fichier deployment s'appelle deployment_react_ashanth.yaml et ce trouve au même endroit que le Dockerfile

## Etape 3 Creer un fichier service.yaml

ici notre fichier deployment s'appelle service_react_ashanth.yaml et ce trouve au même endroit que le Dockerfile