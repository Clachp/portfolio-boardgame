# Projet Portfolio - les jeux de plateau de mon enfance

Ce projet est une API rest pour gérer une collection de jeux de société

## Stack technique

- [NodeJS] (https://nodejs.org/en/download/) (v12 ou supérieur)
- [postgreSQL] (https://www.postgresql.org/download/) (v12 ou supérieure)
- [Sqitch](https://sqitch.org/download/) (v1 ou supérieur)

Ces outils sont nécessaires à l'installation et au fonctionnement de l'API.
À installer sur votre hôte avant de continuer

## Installation

Cloner le dépôt en local

```bash
git clone <url_du_dépôt>
```
Puis dans le dossier local, installer les dépendances npm 

```bash
npm install
```
Copier le fichier .env.example, le renommer en .env et remplir les informations nécessaires

Copier le fichier sqitch.conf.example et le renommer en sqitch.conf 

Enfin, créer une base de donénes PostgreSQL et déployer le projet sqitch dessus

```bash
createdb boardgame
sqitch deploy
```

Configurer PostgreSQL (ou fournir les variables d'environnement nécessaires pour que les commandes 'createdb' et 'sqitch puissent s'exécuter correctement )

## Données de démonstration

Afin de mettre en place quelques données de test, lancer 

```bash
psql -d boardgame -f ./data/seeding.sql
```

## Lancement 

```bash
npm start
```