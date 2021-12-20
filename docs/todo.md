# Les ingrédients d'une bonne API, dans l'ordre :

- Définir le sujet du projet
- MCD
- Conception de la BDD (DDL) : migrations sqitch
- Seeding des tables
- Le serveur web :
  - point d'entrée : index.js
  - router
  - contrôleur(s)
  - modèle(s)
  - connection BDD
- Faire vivre la BDD avec des nouvelles migrations de views, domains, fonctions...
- Doc de l'API : Swagger et JSDoc
- README bien à nous, la vitrine du projet :
  - Que fait notre code
  - stack technique
  - comment installer et lancer le projet
  - infos nécessaires pour utiliser le projet 