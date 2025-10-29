# Qu’est-ce qu’un tableau ?

*-* Un tableau est une structure de données qui permet de stocker plusieurs valeurs dans une seule variable.
*-* Chaque valeur dans un tableau est accessible via un index, qui est un numéro indiquant la position de la valeur dans le tableau.
*-* En JavaScript, les tableaux sont dynamiques et peuvent contenir des éléments de types différents.

```javascript
**1- Créer un tableau: **


let produits = ["Pain", "Lait", "Riz", "Savon"];

**2- Accéder à un élément: **

console.log(produits[0]); // Pain
console.log(produits[2]); // Riz

**3- Modifier un élément: **

produits[1] = "Jus";
console.log(produits); // ["Pain", "Jus", "Riz", "Savon"]

**4- Ajouter un élément: **

  *Ajouter à la fin:* produits.push("Sucre");
  *Ajouter au début:* produits.unshift("Beurre");

**5- Supprimer un élément: **

  *Supprimer à la fin:* produits.pop();
  *Supprimer au début:* produits.shift();

**6- Longueur du tableau: **

console.log(produits.length);

**7- Parcourir un tableau avec une boucle for: **

for (let i = 0; i < produits.length; i++) {
  console.log(produits[i]);
}

**8- Parcourir un tableau avec for...of: **

for (let p of produits) {
  console.log(p);
}

**9- Parcourir un tableau avec for...in: **

for (let index in produits) {
  console.log(produits[index]);
}

```

## Méthodes utiles sur les tableaux

- `push(element)`: Ajoute un élément à la fin du tableau.
- `pop()`: Supprime le dernier élément du tableau et le retourne.
- `shift()`: Supprime le premier élément du tableau et le retourne.
- `unshift(element)`: Ajoute un élément au début du tableau.
- `splice(index, count)`: Supprime `count` éléments à partir de `index`.

```js
  let arr = [1, 2, 3, 4];
  arr.splice(1, 2); // arr devient [1, 4]
  console.log(arr);
  /*
    explication de Splice:
    La méthode splice() modifie le tableau d'origine en supprimant ou en remplaçant des éléments existants
    et/ou en ajoutant de nouveaux éléments à la place.
    Dans cet exemple, nous avons supprimé 2 éléments à partir de l'index 1.
  */
```

- `slice(start, end)`: Retourne une copie d'une portion du tableau.
- `indexOf(element)`: Retourne l'index de la première occurrence de l'élément, ou -1 s'il n'est pas trouvé.

```js
  let arr = ['a', 'b', 'c', 'd'];
  console.log(arr.indexOf('c')); // 2
  console.log(arr.indexOf('x')); // -1
  // indexOf sert à trouver la position d’un élément
```

- `includes(element)`: Retourne true si l'élément est dans le tableau, sinon false.

```js
  let arr = [1, 2, 3, 4];
  console.log(arr.includes(3)); // true
  console.log(arr.includes(5)); // false
  // includes sert à vérifier la présence d’un élément
```

- `join(separator)`: Concatène tous les éléments du tableau en une chaîne, séparés par `separator`.

```js
  let arr = ['Hello', 'World'];
  console.log(arr.join(' ')); // "Hello World"
  // join sert à créer une chaîne à partir des éléments du tableau
  // l’espace entre les guillemets est le séparateur on peut le remplacer par ce qu’on veut
  
```

- `sort()`: Trie les éléments du tableau.

```js
  let arr = [3, 1, 4, 2];
  arr.sort();
  console.log(arr); // [1, 2, 3, 4]
  // sort sert à trier les éléments du tableau
```

- `reverse()`: Inverse l'ordre des éléments dans le tableau.

```js
  let arr = [1, 2, 3];
  arr.reverse();
  console.log(arr); // [3, 2, 1]
  // reverse sert à inverser l’ordre des éléments du tableau
```

- `filter()`: Crée un nouveau tableau avec les éléments qui passent un test.

```js
  let arr = [1, 2, 3, 4, 5];
  let evenNumbers = arr.filter(num => num % 2 === 0);
  console.log(evenNumbers); // [2, 4]
  // filter sert à filtrer les éléments selon une condition
  // num est chaque élément du tableau
```

- `map()`: Crée un nouveau tableau avec les résultats de l'appel d'une fonction sur chaque élément.

```js
  let arr = [1, 2, 3];
  let squared = arr.map(num => num * num);
  console.log(squared); // [1, 4, 9]
  // map sert à transformer les éléments du tableau
  // num est chaque élément du tableau
```

- `reduce()`: Réduit le tableau à une seule valeur en appliquant une fonction.

```js
  let arr = [1, 2, 3, 4];
  let sum = arr.reduce((accumulator, current) => accumulator + current, 0);
  console.log(sum); // 10
  // reduce sert à accumuler les valeurs du tableau en une seule valeur
  // accumulator est la valeur accumulée jusqu’à présent
  // current est la valeur actuelle du tableau
  // initialValue est la valeur initiale fournie (0 dans cet exemple)
```

- `forEach()`: Exécute une fonction pour chaque élément du tableau.

```js
  let arr = ['a', 'b', 'c'];
  arr.forEach((element, index) => {
    console.log(`Index: ${index}, Element: ${element}`);
  });
  /*
    Index: 0, Element: a
    Index: 1, Element: b
    Index: 2, Element: c
  */
  // forEach sert à itérer sur chaque élément du tableau
  // element est chaque élément du tableau
  // index est la position de l’élément dans le tableau
```

- `concat()`: Fusionne deux ou plusieurs tableaux.

```js
  let arr1 = [1, 2];
  let arr2 = [3, 4];
  let merged = arr1.concat(arr2);
  console.log(merged); // [1, 2, 3, 4]
  // concat sert à fusionner plusieurs tableaux en un seul
```

### les tableaux multidimensionnels
