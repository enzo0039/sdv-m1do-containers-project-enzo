# Projet Docker avec API en Rust et Frontend en Next.js

Ce projet utilise Docker pour exécuter une API développée en Rust et un frontend en Next.js. Suivez les instructions ci-dessous pour configurer et exécuter le projet sur votre machine.

## Prérequis

Assurez-vous d'avoir les éléments suivants installés sur votre machine :

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Cloner le dépôt

Clonez le dépôt GitHub sur votre machine :

```bash
git clone https://github.com/enzo0039/sdv-m1do-containers-project-enzo.git
cd sdv-m1do-containers-project-enzo
Configuration de l'environnement
Avant de lancer le projet, assurez-vous d'avoir configuré vos variables d'environnement si nécessaire (voir .env ou autres fichiers de configuration).

Lancer le projet
Pour démarrer l'application, exécutez la commande suivante dans le répertoire du projet :

bash
Copier le code
docker-compose up --build
Cette commande :

Construit les images Docker pour l'API et le frontend.
Démarre les conteneurs.
Accéder à l'application
L'API sera accessible à l'adresse http://localhost:8000.
Le frontend sera accessible à l'adresse http://localhost:3000.
Arrêter le projet
Pour arrêter les conteneurs, utilisez la commande suivante :

bash
Copier le code
docker-compose down
Déploiement CI/CD
Ce projet est configuré avec GitHub Actions pour automatiser le processus de construction et de déploiement. Chaque fois que vous poussez des modifications sur la branche main, une nouvelle image Docker est construite et poussée vers Docker Hub.

