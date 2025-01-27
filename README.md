# Business case: Market Price Retail

## 📜 Contexte  
Vous êtes analyste de données pour une grande entreprise de vente au détail. Le service commercial dispose d'une grande quantité de données sur les coûts et les bénéfices à travers le monde.  
Ils souhaitent explorer et se concentrer sur un marché spécifique et prometteur (car ils constatent une augmentation des bénéfices). Ils ont également besoin de traiter les retours des clients. Votre objectif est d'explorer, de présenter et de cibler un marché.

---

## 🎯 Objectif  
Quelles actions l'entreprise peut-elle entreprendre pour réduire les coûts et augmenter les bénéfices ?  

---

## 📂 Contenu  

Le jeu de données est composé de **8048 lignes**, représentant des commandes associées à leurs clients et produits. Pour chaque client, vous avez le segment correspondant (*Home Office*, *Consumer*, *Corporate*), la catégorie et la sous-catégorie (Papier, Art, photocopieurs, etc.). Pour chaque produit, vous avez le nom, la remise, les ventes, le bénéfice et la quantité.  

---

## 🛠️ Méthodologie  

1. [Analyse et Prétraitement des Données](./notebook.ipynb)  
2. [Définition des KPI](./kpi.md)  
3. Développement d'un tableau de bord  

---

## 🔢 Description du jeu de données  

- ***8048*** : Nombre de clients dans le jeu de données  
- **Description des colonnes** :  

  - **Order ID** : Identifiant unique de chaque commande  
  - **Order Date** : Date de la commande  
  - **Customer Name** : Nom du client  
  - **Country** : Pays du client avec la précision suivante :  
  - **State** : État/province  
  - **City** : Ville  
  - **Region** : Région  
  - **Segment** : Classification du client :  
    - *Home Office* : Ce segment correspond à des auto entrepreneurs ou à de petites entreprises travaillant depuis chez eux.  
    - *Consumer* : Ce segment regroupe des clients individuels achetant pour un usage personnel.  
    - *Corporate* : Ce segment englobe les entreprises ou les grandes organisations passant des commandes en gros.  
  - **Ship Mode** : Mode de livraison utilisé pour la commande  
  - **Category** : Catégorie générale du produit avec la précision suivante :  
  - **Sub-Category** : Sous-catégorie du produit  
  - **Product Name** : Nom du produit  
  - **Discount** : Valeur de la remise en $  
  - **Sales** : Revenu total généré par la transaction, avant toute remise ou marge bénéficiaire.  
  - **Profit** : Montant de l'argent gagné sur la vente  
  - **Quantity** : Quantité de produit dans la commande  
  - **Feedback?** : (Booléen) Le client a-t-il laissé un retour ?  



## 📂 Structure du dépôt
```
CampusCARE/
├── donnees/                # Contient les données brutes et transformées
│   ├── brutes/             # Données brutes (non modifiées)
│   ├── nettoyees/          # Données nettoyées ou modifiées
├── scripts/                # Scripts Python pour le traitement, l'analyse et la modélisation
├── notebooks/              # Notebooks pour l'exploration et la visualisation des données
├── streamlit/              # Code pour l'interface utilisateur
├── dataviz/                # Graphiques, visualisations et rapport final
├── docs/                   # Documentation, Méthodologie
├── images/                 # Visuels, Captures d'écran, logos
└── README.md               # Description du projet
```

## 💡 Conclusion

Au-delà de l’aspect technique, ce business case, bien que fictif, aborde un enjeu humain profond : la santé mentale des étudiants. Il rappelle l’importance de mettre les données au service d’actions concrètes et ciblées pour améliorer le bien-être collectif.

Un projet qui conjugue technique et sens, et qui restera marquant !

---

## 📜 Licence
- [**MIT**](./LICENSE)
