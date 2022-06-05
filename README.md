# Projet 5 : Segmentez des clients d'un site e-commerce

Parcours Data Scientist d'OpenClassrooms en partenariat avec CentraleSupélec.

L'objectif du projet est d'effectuer la segmentation des clients de l'entreprise Olist (e-commerce) grâce à l'analyse des données, des comportements et de proposer un contrat de maintenance basée sur l'analyse de la stabilité des segments au cours du temps.

Le jeu de données est constitué de 9 fichiers de données clients comportant :
- Les caractéristiques des clients ;
- Les dates et statuts des commandes ;
- Les prix des articles et des livraisons ;
- Les moyens de paiement et le montant total des commandes ;
- Les niveaux de satisfaction des clients ;
- Les caractéristiques des produits ;
- Les caractéristiques des vendeurs ;
- Les catégories des articles ;
- Les données de géolocalisation.

La source des données est la suivante : https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce


## Les étapes de l'analyse exploratoire :
- L'import et le nettoyage du jeu de données ;
- L'utilisation de la segmentation RFM en marketing permettant de classer les clients en fonction de 3 critères :
  - La Récence ;
  - La Fréquence ;
  - Le Montant des achats.
- La prise en compte de la satisfaction des clients (review score) ;
- Le feature engineering et l'exploration du jeu de données ;
- L'analyse univariée (distributions des variables, test d'adéquation des variables à une loi normale et test d'égalité des variances) ; 
- L'analyse multivariée :
  - L'analyse des corrélations entre les variables quantitatives ;
  - L'analyse bivariée entre les variables quantitatives et catégorielles ;
  - L'analyse de la variance par la méthode ANOVA.
- La réduction de dimension (PCA).


## Les étapes des essais des différentes approches de modélisation :
- L'import des données et feature engineering (sélection des variables pertinentes et des subsets) ;
- Les essais des différents algorithmes de clustering (classification non supervisée) et sélection du modèle adapté au problème métier :
  - Le KMeans ;
  - Le clustering hiérarchique ;
  - Le DBSCAN ;
  - Le K-Prototypes.
- La segmentation de l'ensemble des clients en matière de commandes et de satisfaction.


## Les étapes de la simulation pour déterminer la fréquence nécessaire de mise à jour du modèle de segmentation :
- L'import des données et le feature engineering (sélection des variables pertinentes) ;
- La segmentation des clients sur un mois d'une période d'un an (les 12 derniers mois) ;
- L'analyse de la stabilité des segments par mois sur les 12 derniers mois.
