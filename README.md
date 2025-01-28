# Business case: Market Price Retail

## 📜 Contexte  
Vous êtes analyste de données pour une grande entreprise de vente au détail. Le service commercial dispose d'une grande quantité de données sur les coûts et les bénéfices à travers le monde.  
Ils souhaitent explorer et se concentrer sur un marché spécifique et prometteur (car ils constatent une augmentation des bénéfices). Ils ont également besoin de traiter les retours des clients. 
Votre objectif est d'explorer, de présenter et de cibler un marché.

---

## 🎯 Objectif  
Quelles actions l'entreprise peut-elle entreprendre pour réduire les coûts et augmenter les bénéfices ?  

---

## 📂 Contenu  

Le jeu de données est composé de **8048 lignes**, représentant des commandes associées à leurs clients et produits. Pour chaque client, vous avez le segment correspondant (*Home Office*, *Consumer*, *Corporate*), la catégorie et la sous-catégorie (Papier, Art, photocopieurs, etc.). Pour chaque produit, vous avez le nom, la remise, les ventes, le bénéfice et la quantité.  

---

## 🛠️ Méthodologie  

1. [Analyse et Prétraitement des Données](./docs/recherche/notebook.ipynb)  
2. [Définition des KPI](./docs/recherche/kpis.md)  
3. [Développement d'un tableau de bord](./livrables/BC_MPR.pbix)
4. [Mise en place d'un PowerPoint de présentation](./livrables/BC_MPR.pptx)

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



## 🏗️ Structure du dépôt
```
BC_MARKET_RETAIL/
├── docs/                   # Contient les documents non livrables et images
│   ├── images/             # Toutes les images utilisées dans les livrables
│   ├── recherche/          # Notebook de nettoyage et exploration des données et réflexion sur les kpis
├── donnees/                # Contient les données brutes et transformées
│   ├── brutes/             # Données brutes (non modifiées)
│   ├── nettoyees/          # Données nettoyées et modifiées
├── livrables/              # Contient tout ce qui a été demandé et qu'il faudra rendre
│   ├── dashboard/          # Dashboard powerBI
│   ├── presentation/       # owerpoint de présentation
└── README.md               # Description du projet
```

## 🏁 Conclusion

- Il faut agir rapidement sur les marchés qui ont un discount moyen trop élevé qui engendrent de lourdes pertes pour l’entreprise.
- On peut voir que des pays qui apportent un fort CA ont des taux de discount assez bas. Une bonne stratégie serait de diminuer les remises des pays ou le bénéfice est négatif pour en apporter plus aux marchés qui sont déjà porteur pour les fidéliser  définitivement et aller chercher le chiffre chez eux car ce sont eux qui portent l’entreprise.
- Se focaliser sur les produits technologiques qui apportent le plus de chiffre pour des ventes beaucoup moins importantes permettra de gonfler le chiffre.
- On sait que l’entreprise reçoit beaucoup de feedback de la part de ses clients, lui permettant d’avoir des avis représentatifs sur leur expérience qui sont très importants à exploiter.


---

## 📜 Licence
- [**MIT**](./LICENSE)
