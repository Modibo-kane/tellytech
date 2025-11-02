# Partie 1 – Tableaux d’objets + méthodes combinées

**Exercice 1** – Produits en promotion

On te donne un tableau :

let produits = [
  { nom: "Pain", prix: 150 },
  { nom: "Lait", prix: 500 },
  { nom: "Savon", prix: 300 },
  { nom: "Riz", prix: 700 },
  { nom: "Sucre", prix: 800 }
];

 Crée un nouveau tableau contenant seulement les produits à moins de 500 FCFA
(utilise filter())

**Exercice 2** – Augmentation de prix

Augmente le prix de tous les produits de 10%
(utilise map() et calcule un prix mis à jour)

**Exercice 3**  – Trouver le produit le plus cher

Affiche le produit le plus cher du magasin
(utilise sort() ou une boucle)

**Exercice 4** – Supprimer un produit par son nom

Demande à l’utilisateur de saisir le nom d’un produit
→ s’il existe, supprime-le du tableau
→ sinon, affiche “Produit pas trouvé”

## Partie 2 – Analyse de données

**Exercice 5** – Statistiques du magasin

Affiche :

Le prix moyen

Le prix le plus petit

Le prix le plus grand

une seule boucle autorisée

**Exercice 6** – Recherche intelligente

Demande à l’utilisateur un texte

Affiche tous les produits dont le nom contient cette recherche (ex : “a” → Pain, Savon…)

→ utilise .includes() + filter()

**Exercice 7** – Classement des produits

Trie le tableau selon le nom (ordre alphabétique A → Z)

**Exercice 8**   – Format affichage catalogue

Affiche chaque produit sous la forme :

1 - Pain : 150 FCFA
2 - Lait : 500 FCFA
...

→ Numérotation automatique avec forEach()

### Partie 3 – Algorithmes avec tableaux

**Exercice 9** – Suppression des doublons

À partir du tableau :

let a = [1,2,3,3,4,5,5,6,7];

Créer un nouveau tableau sans doublon

**Exercice 10** – Fusionner deux magasins

On te donne :

let magasin1 = ["Pain", "Lait", "Sel"];
let magasin2 = ["Savon", "Lait", "Riz"];

Créer un tableau contenant tous les produits sans doublons

**Exercice 11** – Trouver les produits en commun

Affiche les éléments présents dans les deux tableaux ci-dessus

**Exercice 12** – Réorganiser les stocks

Demande à l’utilisateur deux positions : i et j
Échange les éléments correspondant dans le tableau

Ex :

Avant : ["Pain", "Lait", "Riz"]
Entrée : i=0 et j=2
Résultat : ["Riz", "Lait", "Pain"]

#### Partie 4 – Mini Projet “Magasin Pro”

**Mini-Projet :** Gestion avancée

Créer un programme menu-interactif :

1. Afficher stock complet
2. Rechercher par nom
3. Ajouter un produit
4. Supprimer un produit
5. Afficher produits à moins de 500 FCFA
6. Trier par prix (croissant)
7. Quitter
