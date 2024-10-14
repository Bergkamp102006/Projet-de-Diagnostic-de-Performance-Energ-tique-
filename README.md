# Projet de Diagnostique dePerformance Energétique (DPE) sur les logements du Rhône
L'application Tableau de Bord DPE permet d'explorer, visualiser et analyser les données des diagnostics de performance énergétique (DPE) des logements du département du Rhône. Elle est divisée en plusieurs pages qui offrent des fonctionnalités variées telles que la visualisation des données sous forme de tableaux, graphiques et cartes géographiques interactives. L'utilisateur peut naviguer à travers différents onglets pour accéder à ces fonctionnalités.

Les données sont issues de l'Adème via le lien suivant : https://data.ademe.fr/datasets/dpe-v2-logements-existants/api-doc
Les données traitées dans cette application shiny sont filtrées sur les codes postaux du Rhône.

1- Documentation technique :
  Schéma de l'architecture de l'application
  Suivi pour l'installation de l'application
  Packages nécessaires
  Mise en forme et rédaction

2- Documentation fonctionnelle 
Les pages du menu :
  2.1.Page Documentation:
    
    Présente un aperçu descriptif des données utilisées dans l'application.
  
  2.2.Page Tableau de Données:
   
    Un tableau interactif (DataTable) affiche une description des principales variables présentes dans le fichier DPE
  
  2.3.Page Statistiques:
   
    Offre une vue d'ensemble des statistiques importantes liées aux DPE, y compris la répartition des étiquettes DPE, des coûts de chauffage, ainsi qu'un résumé statistique
  
  2.4.Page Carte:
    
    Permet de géocoder un code postal saisi par l'utilisateur et d'afficher le résultat sur une carte interactive.

3- Vidéo explicative de l'installation de l'application en local


Lien de l'application shiny : https://murielmesmin.shinyapps.io/greenapplication/
