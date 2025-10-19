# Introduction – Les conditions et boucles en JavaScript

## 1. Les conditions

🔹**if– la condition simple**

```js
    let age = 18;

    if (age >= 18) {
    console.log("Tu es majeur");
    }

    // Si la condition est vraie, le bloc s’exécute.
```

🔹 **if ... else – avec une alternative**

```js
  let temperature = 25;

  if (temperature > 30) {
    console.log("Il fait chaud !");
  } else {
    console.log("Il fait frais !");
  }

  // Si la première condition est fausse, c’est le else qui s’exécute.

```

🔹 if ... else if ... else – plusieurs cas possibles

```js
  let note = 14;

  if (note >= 16) {
    console.log("Excellent");
  } else if (note >= 10) {
    console.log("Assez bien");
  } else {
    console.log("Insuffisant");
  }

```

🔹 switch – pour plusieurs valeurs fixes

```js

  let jour = "lundi";

  switch (jour) {
    case "lundi":
      console.log("Début de semaine");
      break;
    case "vendredi":
      console.log("Presque le week-end !");
      break;
    default:
      console.log("Jour normal");
  }
    /*  switch est pratique quand on teste une seule variable contre plusieurs valeurs. */

```
