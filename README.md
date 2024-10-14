# 
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


2. Installation de l'application sur votre poste
1- Ouvrir Rshiny
2-install.packages(c("shiny", "httr", "jsonlite", "shinydashboard", "dplyr", "leaflet", "DT", "tidygeocoder", "ggplot2", "geosphere", "maps"))
3 - Télécharger le code et tous les fichiers nécessaires
4-Exécuter le code

II-Documentation Fonctionnelle de l'Application Tableau de Bord DPE

1. Présentation Générale de l'Application
L'application Tableau de Bord DPE permet d'explorer, visualiser et analyser les données des diagnostics de performance énergétique (DPE) des logements du département du Rhône. Elle est divisée en plusieurs pages qui offrent des fonctionnalités variées telles que la visualisation des données sous forme de tableaux, graphiques et cartes géographiques interactives. L'utilisateur peut naviguer à travers différents onglets pour accéder à ces fonctionnalités.


2- Détail des Pages de l'Application
Page 1 : Documentation des Données
Fonctionnalités Majeures
Tableau de Documentation : Présente une description détaillée de chaque variable incluse dans le jeu de données.
Affichage interactif : Le tableau est dynamique, avec des fonctionnalités de tri et de pagination.
Mise en Page
Titre : "Documentation des données"
Contenu : Un tableau interactif affichant deux colonnes, l’une pour le nom de la variable et l’autre pour sa description.
Actions disponibles : Consultation des informations, navigation à travers les pages du tableau


3-Page 2 : Tableau de Données
Filtrage par code postal : Sélectionnez un code postal spécifique pour afficher uniquement les logements situés dans cette zone.
Tableau interactif : Présente les données DPE avec des options de pagination, tri et recherche.
Actualisation des données : Un bouton permet de réinitialiser le filtre pour afficher toutes les données.
Exportation CSV : Les utilisateurs peuvent télécharger les données filtrées sous forme de fichier CSV.
Page 3 : Statistiques DPE

Page 4 : Carte DPE

Répartition des étiquettes DPE : Histogramme montrant la distribution des différentes étiquettes (A à G).
Coûts de chauffage : Histogramme des coûts de chauffage des logements.
Proportions des logements : Diagramme circulaire montrant la répartition des logements par code postal.
Nuage de points (Scatter plot) : Visualise la relation entre le coût total des usages et le code postal.

Page 4 : Carte DPE

Géocodage : L'utilisateur peut saisir un code postal pour géocoder l'emplacement.
Carte interactive : Utilisation de leaflet pour afficher les résultats sur une carte. Les utilisateurs peuvent zoomer et interagir avec la carte.
Affichage des marqueurs : Après géocodage, un marqueur est ajouté à la carte à l'emplacement correspondant au code postal entré.
