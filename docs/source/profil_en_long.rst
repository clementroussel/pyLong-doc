Profils en long - généralités et méthodes
*****************************************

Définitions
===========

Point de vue hydromorphologique
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

    Le profil en long d’un cours d’eau est une représentation graphique qui met en rapport la cote du fond du lit et/ou de la ligne d’eau et/ou du niveau des berges (en ordonnées), et 
    la distance (en abscisses). Il peut être réalisé à différentes échelles du cours d’eau (linéaire complet, tronçons, stations) et permet d’observer les variations longitudinales de 
    la pente du fond du lit et/ou de la ligne d’eau et/ou du niveau des berges. 
    
    C’est un outil hydromorphologique essentiel qui traduit, par la comparaison diachronique de plusieurs relevés, les processus physiques verticaux d’ajustement (érosion/dépôt), 
    sous l’effet notamment des variations de débits liquide et solide (variables de contrôle primaires). Plus localement, la pente et la géométrie de la vallée, la granulométrie du lit 
    et la végétation rivulaire (variables de contrôle secondaires) influencent aussi la forme du profil longitudinal. 

    (source : https://professionnels.ofb.fr/ - Guide pour l'élaboration de suivis d'opérations de restauration hydromorphologique en cours d'eau - Mai 2019)

Méthodes de génération d'un profil en long
==========================================

Avec QGIS
---------

Utilisation de la BD TOPO® de l'IGN
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

La BD TOPO® de l'IGN possède une couche nommée *TRONCON_HYDROGRAPHIQUE*, classée dans la thématique *HYDROGRAPHIE*, qu'il est possible d'exploiter pour
construire un profil en long.

1. Téléchargement de la BD TOPO® depuis le portail https://geoservices.ign.fr/bdtopo
2. Chargement de la couche *TRONCON_HYDROGRAPHIQUE* dans QGIS
3. Sélection manuelle des tronçons d'intérêt
4. Enregistrement de la sélection dans une nouvelle couche
5. Regroupement des tronçons (*regrouper* / *dissolve*)
6. Suppression de tous les champs de la table attributaire (*supprimer champ(s)* / *drop fields*)
7. Ajout d'un champ auto-incrémenté "Id" (*ajouter un champ auto-incrémenté* / "add autoincrement field*)
8. Utilisation du script *Polyline Projection*

Avantages:
- Rapidité - simplicité
- Aucun MNT requis car la donnée altimétrique est contenue dans les entités de la couche *TRONCON_HYDROGRAPHIQUE*

Inconvévients:
- Origine, qualité des données altimétriques de la couche *TRONCON_HYDROGRAPHIQUE*

Utilisation des courbes de niveaux
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Utilisation de profils en travers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Utilisation des algorithmes de la librairie SAGA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Projection sur un axe de référence
==================================



