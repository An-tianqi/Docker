# Docker
Ce projet permettre de deployer simplement une application à l'aide de conteneurs Docker 

D'abord assurez vous que Docker est bien installé

Ensuit bash Copy code git clone https://github.com/An-tianqi/Docker.git

docker-compose up --build

Cette commande créera les images Docker pour votre application.

Accédez à http://localhost:5000 pour afficher votre application.

docker-compose down

Cette commande pour arreter l'application

# Workflows

# Structur

Frontend : l'application frontend React.
App : l'application backend Flask.
DB : les scripts SQL pour configurer la base de données MySQL.
Docker-compose.yml : Définit la configuration multi-conteneurs avec Docker Compose.

# Application

Construis l'image Docker à partir du Dockerfile :

docker build -t react

Exécute le conteneur Docker :

docker run -p 8080:80 react

# Test

Le test backend exécuter par la commande act (pytest).

# Schéma 


# Configuration Docker Compose

La configuration Docker Compose orchestre le déploiement de l'application complète, incluant l'API Flask, la base de données MySQL, l'application React, et un serveur Nginx comme reverse proxy.

# Services

back : API Flask il avait deux routes index et delete

# Conclu

Cette documentation offre un aperçu de la structure et des fonctionnalités de projet, les commandes Docker/Docker Compose. C'est un guide utile pour les développeurs et les utilisateurs finaux souhaitant comprendre et interagir avec votre application.