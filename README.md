#  Catalogue LEGO – Documentation du projet

## 📌 Présentation générale

Le projet **Catalogue LEGO** est une application web permettant de consulter, gérer et acheter des sets LEGO.

L’application propose un catalogue interactif regroupant de nombreux ensembles avec leurs informations détaillées. Elle permet également aux utilisateurs d’interagir dynamiquement avec les produits via différentes fonctionnalités (recherche, tri, panier, modification…).

---

##  Objectifs du projet

* Développer une interface web moderne et intuitive
* Mettre en place un catalogue dynamique de produits
* Implémenter des fonctionnalités interactives (tri, recherche, filtres)
* Gérer un système de panier utilisateur
* Permettre la gestion complète des produits (CRUD)

---

##  Environnement technique

Le projet repose sur les technologies suivantes :

* Vue.js
* JavaScript (ES6+)
* HTML5
* CSS3
* Node.js / npm


## 📁 Structure du projet

```
Catalogue-LEGO/
│
├── public/
│   ├── img/
│   ├── favicon.ico
│   ├── index.html
│   └── Journal.md
│
├── src/
│   ├── assets/
│   │   └── logo.png
│   │
│   ├── components/
│   │   └── HelloWorld.vue
│   │
│   ├── router/
│   │   └── index.js
│   │
│   ├── store/
│   │   └── index.js
│   │
│   ├── views/
│   │   ├── AboutView.vue
│   │   └── HomeView.vue
│   │
│   ├── App.vue
│   └── main.js
│
├── package.json
├── package-lock.json
├── babel.config.js
├── vue.config.js
└── README.md
```

---

##  Organisation de l’interface

Le fichier `index.html` constitue le point central de l’interface utilisateur.

### 📄 Structure détaillée du fichier

* **Lignes 9 à 786 :**
  Définition des styles CSS (mise en page, animations, thèmes…)

* **Lignes 791 à 803 :**
  Barre de navigation (Navbar) :

  * Logo
  * Mode jour / nuit
  * Accès au panier

* **Lignes 805 à 974 :**
  Zone de gestion des produits :

  * Tri par prix (croissant / décroissant)
  * Filtrage par thème
  * Barre de recherche dynamique
  * Ajout d’un produit
  * Mode grille / liste

* **Lignes 1088 à 1387 :**
  Cartes des produits :

  * Affichage des sets LEGO
  * Informations détaillées
  * Actions (modifier, supprimer, ajouter au panier)

---

## 🚀 Fonctionnalités principales

###  Catalogue produits

Chaque produit contient :

* Nom
* Prix
* Référence
* Nombre de pièces
* Thème
* Stock
* Description
* Image

---

### 🎨 Thèmes disponibles

* Harry Potter
* Disney
* Fleurs
* Mario
* Animaux

---

### 🔍 Recherche et filtres

* Recherche dynamique en temps réel
* Filtrage par thème
* Tri :

  * Prix croissant
  * Prix décroissant

---

###  Affichage

* Mode grille
* Mode liste

---

### 🛒 Panier

* Ajout d’articles
* Consultation du panier

---

###  Gestion des produits

* Ajout d’un nouveau set (avec image)
* Modification des caractéristiques
* Suppression d’un produit
* Affichage des détails

---

### 🌙 Interface utilisateur

* Mode jour / nuit

---

## ⚠️ Problèmes rencontrés

Certaines fonctionnalités présentent des comportements inattendus nécessitant une analyse.


###  Barre de recherche

Lors de la saisie dans la barre de recherche, l’interface devient instable. L’écran présente des mouvements anormaux accompagnés d’un déclenchement sonore non attendu.


###  Ajout au panier

L’ajout d’un article au panier entraîne l’apparition simultanée de nombreuses fenêtres d’erreur.
La fermeture de ces fenêtres ne semble pas effective, celles-ci réapparaissant immédiatement.
Certains éléments de fermeture sont difficilement accessibles ou non fonctionnels.


###  Modification d’un produit

Lors de la modification d’un produit, un élément visuel inattendu apparaît et perturbe fortement l’interaction avec l’interface.


###  Mode nuit

L’activation du mode nuit entraîne l'ouverture d'une page de redémarrage rendant le clavier inutilisable et empêchant toute utilisation de cette fonctionnalité.


###  Recherche de produits

Certains produits ne sont pas correctement retournés selon la saisie utilisateur (ex : différence majuscule/minuscule), ce qui entraîne des résultats incomplets.


---

## 📈 Améliorations attendues

* Stabilisation de l’interface
* Correction des erreurs bloquantes
* Amélioration de la recherche
* Fiabilisation des interactions utilisateur
* Optimisation globale des performances

---

## 👥 Équipe projet

* Adi Katia
* Luce-Dubas Léna
* FEHA Hermann Junior
* Touazi Yacine

---
