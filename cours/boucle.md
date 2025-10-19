# 2. Les boucles

**Les boucles permettent de répéter un bloc d’instructions plusieurs fois.**

2.1 **for (pour)**

```js
// Quand on sait combien de fois on veut répéter :

for (let i = 1; i <= 5; i++) {
  console.log("Tour numéro " + i);
}

// Démarre à 1, répète tant que i <= 5, et incrémente à chaque tour.

```

2.2 **while (tant que)**

```js
//Quand on ne sait pas à l’avance combien de fois répéter :

let nombre = 1;

while (nombre <= 5) {
  console.log("Compteur : " + nombre);
  nombre++;
}

//La boucle s’exécute tant que la condition est vraie.

```

---
2.3 **do...while (faire...tant que)**

```js
//La boucle s’exécute au moins une fois, même si la condition est fausse :

let n = 0;

do {
  console.log("Essai numéro " + n);
  n++;
} while (n < 3);

```
