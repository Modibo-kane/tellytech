# LES BASES DES BASES POUR COMMENCER JS

1. **Opérateurs arithmétiques**
   let a = 10;
   let b = 3;
   console.log(a + b); // addition
   console.log(a - b); // soustraction
   console.log(a \* b); // multiplication
   console.log(a / b); // division
   console.log(a % b); // modulo (reste)

2. **Opérateurs d’affectation**

   let x = 5;
   x += 2; // équivaut à x = x + 2
   x -= 1; // équivaut à x = x - 1

   ---
3. **Opérateurs de comparaison**

   console.log(5 == "5");  // true (égalité de valeur)
   console.log(5 === "5"); // false (égalité stricte : type + valeur)
   console.log(5 != 3);    // true
   console.log(5 !== "5"); // true
   console.log(4 > 3);     // true
   console.log(4 <= 2);    // false

   ---
4. **Opérateurs logiques**

   console.log(true \&\& false); // ET
   console.log(true || false); // OU
   console.log(!true);         // NON

   ---
5. **Les concaténations et les template literals**

   let nom = "Modibo";
   let age = 25;

   // ancienne méthode
   console.log("Bonjour " + nom + ", tu as " + age + " ans.")

   // nouvelle méthode (template literal)
   console.log(`Bonjour ${nom}, tu as ${age} ans.`);

   ---
6. **La conversion de types**

    Quand on utilise prompt(), les valeurs sont des chaînes :
     let x = prompt("Entrez un nombre :");
     console.log(typeof x); // string

     x = Number(x); // conversion en nombre
     console.log(typeof x); // number

   *ON peut pas comparer deux élément de type different*

   ---
7. **Les valeurs booléennes**

 let estMajeur = true

 if (estMajeur) {
   console.log("Tu peux voter !")
    };
