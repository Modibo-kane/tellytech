# Qu’est-ce qu’un objet ?

Un objet est une structure de données qui permet de stocker plusieurs informations liées entre elles sous forme clé : valeur.

Par exemple, pour représenter un produit dans un magasin, on peut utiliser un objet avec des propriétés comme le nom, le prix et la quantité :

```javascript
let produit = {
  nom: "Pain",
  prix: 150,
  quantite: 30,
  categorie: "Alimentaire"
};

ici *nom*, *prix*, *quantite* et *categorie* sont des clés (ou propriétés) de l’objet, et "Pain", 150, 30 et "Alimentaire" sont les valeurs associées à ces clés.

```

## Accéder aux propriétés

On peut accéder aux valeurs des propriétés d’un objet en utilisant la notation par point ou la notation par crochets :

```javascript
**a- Avec le point .**
console.log(produit.nom); // Notation par point

**b- Avec les crochets [ ]**
console.log(produit["prix"]); // Notation par crochets

```

### Modifier une propriété

On peut également modifier les valeurs des propriétés de la même manière :

```javascript
produit.nom = "Baguette"; // Modification avec le point
produit["prix"] = 200; // Modification avec les crochets

```

#### Ajouter / Supprimer une propriété

```javascript

// Ajouter une propriété
produit.stock = 50;
console.log(produit.stock); // 50

// Supprimer une propriété
delete produit.categorie;
console.log(produit);
```

## Parcourir les clés de l’objet → for...in

```javascript
for (let cle in produit) {
  console.log(cle + " : " + produit[cle]);
}

```

## Objets imbriqués

```javascript
let commande = {
  id: 1,
  produit: {
    nom: "Pain",
    prix: 150
  },
  client: {
    nom: "Alice",
    age: 30
  }
};

console.log(commande.produit.nom); // Pain
console.log(commande.client.age); // 30
```

## Tableaux d’objets

Un tableau d’objets est une liste où chaque élément est un objet. Par exemple, un tableau de produits :

```javascript
let produits = [
  { nom: "Pain", prix: 150, quantite: 30 },
  { nom: "Lait", prix: 100, quantite: 20 },
  { nom: "Riz", prix: 200, quantite: 10 }
];

console.log(produits[0].nom); // Pain
console.log(produits[1].prix); // 100
console.log(produits[2].quantite); // 10
```

-*Rechercher dans un tableau d’objets*
<!-- Trouver un produit par son nom  -->

```js
let resultat = produits.find(p => p.nom === "Lait");
console.log(resultat);
```

-*Filtrer selon un prix*

```js
let chers = produits.filter(p => p.prix > 300);
console.log(chers);
```

-*Ajouter un produit dans un tableau d’objets*

```js
produits.push({ nom: "Sucre", prix: 800 });
console.log(produits);
```

### Résumé important

**obj.cle** Lire la valeur
**obj.cle = valeur** Modifier / ajouter
**delete obj.cle** Supprimer
**for...in** Parcourt des propriétés
**this** Référence l’objet actuel
**find, filter** Recherche dans tableaux d’objets

## Petit exercice dans le cours

À partir de cet objet :

let produit = {
  nom: "Riz",
  prix: 600
};

1️ Affiche son nom
2️ Change son prix
3️ Ajoute une propriété stock
4️ Affiche toutes ses propriétés avec for...in
