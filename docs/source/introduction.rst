Introduction
************

.. image:: ./icones/introduction.png
   :align: center
   :scale: 75%
   
|

pyLong, quésaco ?
=================

**pyLong** est un logiciel de visualisation, d'édition, d'analyse et de traitement de profils en long **développé par les Services de Retauration de Terrains en Montagne de l'Office National des Forêts (ONF-RTM) et financé par le Minstère de l'Agriculture et de l'ALimentation (MAA)**. Il a été pensé et conçu pour répondre à des besoins liés aux domaines de l'hydraulique torrentielle et des chutes de blocs en milieu montagneux. 

.. figure:: ./captures/apercu.png
   :align: center
   :scale: 20
   
   Aperçu du logiciel pyLong.
   
**pylong** facilite l'interprétation de profils en long générés à partir de modèles numériques de terrain à haute résolution (LiDAR notamment). Ces profils comportent en effet des milliers de points ce qui rend impossible une interpétation géoémorphologique basée sur l'évolution de la pente longitudinale. **pylong** permet une simplification automatisée et/ou interactive des profils en long et le calcul des petes longitudinales sur des tronçons homgènes d'un point de vue géomrophologique. Les principales fonctionnalités du logiciel sont listées ci-après :

* **Simplification automatisée de profil en long** avec algorithme de Visvalingam & Whyatt [#f1]_ 
* **Simplification interactive du profil en long** avec ajouts ou supprssion de points directement sur le graphique ;
* Filtrage de profil en long avec différents algorithmes de traitement du signal (Butterworth, Lowess, Savitzky-Golay) ;
* Calcul des pentes longitudinales sur profil simplifié ;
* **Tracé facilité de mutilples séries de profils en long et d'annotations** ;
* Fonctionnalités étendues d'affichage et de personnalisation des profils en long : gestion de mises en pages multiples, ajout de subplots de comptraison diagronique de profils en long,...
* **Toolbox de modèles 1D empiriques de propagation de laves torrentielles et de chutes de blocs**. 
* Export de graphique au format .jpg pour insertion dans document d'étude.

.. figure:: ./captures/apercu.png
   :align: center
   :scale: 20
   
   Exemple de profil en long généré avec pyLong.
   

La petite histoire de pyLong
============================

Une première version basée sur des bibliothèques de calul **Python** et interfacée avec Microsoft Excel a vu le jour en 2018. Une version logicielle de **pylong** a été développée en 2020 pour faciliter son usage et sa diffusion en interne aux services ONF-RTM, mais aussi dans l'objectif d'une diffusion en externe auprès des partenaires intéressés (collectivités Gémapiennes, bureaux d'études, recherche). Celle-ci inclut des développements spécifiques non présents dans la version initiale (Toolbox, fonctionnalités étendues d'affichage,...).

A ce jour seule la version logicielle de **pyLong** est maintenue.



À qui s'adresse pyLong ?
========================

**pyLong** a été créé pour des besoins opérationnels par des ingénieurs pour des ingénieurs. Il peut être utilisé par des bureaux d'études, des maitres d'ouvrages, des chercheurs,...

.. [#f1] https://en.wikipedia.org/wiki/Visvalingam%E2%80%93Whyatt_algorithm 
