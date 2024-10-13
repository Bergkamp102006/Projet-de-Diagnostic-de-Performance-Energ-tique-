# Projet-de-Diagnostic-de-Performance-Energ-tique-
DPE dans le Rhône
Documentation Technique de l'Application R Shiny : Tableau de Bord DPE
1. Schéma de l'architecture
L'architecture de l'application est organisée en trois principaux composants :

Interface Utilisateur (UI) : Définit la présentation de l'application, y compris les menus et les différentes sections pour afficher les données, les statistiques et la carte.

Serveur : Gère la logique de l'application, y compris le traitement des données, les graphiques et les actions de l'utilisateur (tels que les filtres et les téléchargements).

Données Globales : Charge et nettoie les données à partir d'un fichier CSV pour être utilisées dans l'application.

+----------------+          +-------------+         +-----------------+
|   Interface     | <-----> |   Serveur   | <-----> |  Données CSV    |
|     Utilisateur |          |             |         |  (resultats_dpe.csv) |
+----------------+          +-------------+         +-----------------+


