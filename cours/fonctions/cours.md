# Introduction : Qu’est-ce qu’une fonction ?

Une *fonction* est un bloc de code `réutilisable` qui effectue une tâche précise.

Exemple dans la vie réelle :
Une fonction, c’est comme une machine à jus. Tu donnes des fruits (les paramètres) et tu obtiens du jus (le résultat)

## Déclaration d’une fonction

`Syntaxe de base`

```js
function nomDeLaFonction() {
  // instructions
}
// Exemple
function direBonjour() {
  console.log("Bonjour !");
}

direBonjour(); // Appel de la fonction

```

### Fonctions avec paramètres

les paramètres permettent de rendre les fonctions plus flexibles et réutilisables.
un paramètre est une variable qui sert à recevoir une valeur lors de l’appel de la fonction.
cela permet de passer des informations à la fonction.
cette valeur peut être utilisée à l’intérieur de la fonction.

```js
function direBonjour(nom) {
  console.log("Bonjour " + nom + " !");
}

direBonjour("Alice"); // Appel de la fonction avec un argument
direBonjour("Bob");
```

### Fonctions avec valeur de retour (return)

```js
Le mot-clé return permet à la fonction de renvoyer un résultat.

function addition(a, b) {
  return a + b;
}

let resultat = addition(3, 5);
console.log(resultat); // 8


💡 Sans return, la fonction ne renvoie rien (elle “fait” juste une action).
```

### Les différents types de fonctions

- **Fonction déclarée**

```js
function carre(x) {
  return x * x;
}
// la forme la plus classique
console.log(carre(4)); // 16
```

- **Fonction anonyme (expression de fonction)**

```js
let carre = function(x) {
  return x * x;
};
// ici la difference avec la fonction declarée c'est qu'on l'assigne a une variable mais on ne lui donne pas de nom
// on l'appelle avec le nom de la variable
console.log(carre(4)); // 16
```

- **Fonction fléchée (arrow function)**

```js
let carre = (x) => x * x;
// ou sans parenthèses si un seul paramètre
let carre = x => x * x;
// on les retrouve souvent dans les functions prédéfine de js comme find(), filter(), map(), foreach() etc...
```

*NB:* Toutes ces versions font la même chose, mais la fléchée est plus courte.

#### Les fonctions avec valeurs par défaut

```js
// Tu peux définir une valeur par défaut si aucun argument n’est donné :

function saluer(nom = "inconnu") {
  console.log("Bonjour " + nom);
}

saluer();         // Bonjour inconnu
saluer("Fatou");  // Bonjour Fatou

```

#### La portée des variables (Scope)

```js
'Locale ': une variable déclarée dans une fonction n’existe que dans cette fonction.

'Globale ': une variable déclarée en dehors d’une fonction est accessible partout.

Exemple :
let x = 10; // variable globale

function afficher() {
  let y = 5; // variable locale
  console.log(x + y);
}

afficher(); // 15
console.log(y); //  Erreur : y n’est pas défini
```

#### Fonctions imbriquées

```js
// Une fonction peut en contenir une autre.

function parent() {
  function enfant() {
    console.log("Je suis à l’intérieur !");
  }
  enfant();
}

parent();// Appel de la fonction parent qui appelle enfant
```

#### Fonctions comme paramètres (callback)

```js
// Une fonction peut être passée en paramètre à une autre fonction.

function saluer(nom, bye) /* ici on a une fonction callback réprésenté par 'bye' au niveau des paramètre  */ 
{
  console.log("Bonjour " + nom);
  bye();// ici on appelle notre fonction callback
}

function auRevoir() /* ici on construit une fonction normale*/
{
  console.log("À bientôt !");
}

saluer("Kane", auRevoir); // On passe la fonction auRevoir comme argument ( valeur) à saluer
```
