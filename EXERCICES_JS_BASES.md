# Série d’exercices – Les bases avant les conditions en JavaScript

Ce document regroupe une série d’exercices progressifs à faire après avoir étudié :

- les opérateurs arithmétiques, d’affectation, de comparaison et logiques
- la concaténation et les template literals
- la conversion de types
- les booléens

---

## Partie 1 – Opérateurs arithmétiques et d’affectation

### Exercice 1 – Calculs simples

Demande à l’utilisateur deux nombres et affiche :

- leur somme
- leur différence
- leur produit
- leur quotient
- le reste de la division  
 Utilise `prompt()` pour les entrées et `Number()` pour la conversion.

---

### Exercice 2 – Mise à jour d’une variable

```js
let compteur = 10;
// 1. ajoute 5
// 2. enlève 2
// 3. multiplie par 3
// 4. affiche le résultat final
```

---

### Exercice 3 – Conversion de monnaie

Demande un montant en francs CFA et affiche l’équivalent en euros (1 euro = 655.957 FCFA).

---

## Partie 2 – Opérateurs de comparaison

### Exercice 4 – Comparer deux nombres

Demande deux nombres et affiche s’ils sont :

- égaux
- différents
- si le premier est plus grand que le second
- ou plus petit.

---

### Exercice 5 – Égalité stricte

Crée deux variables :

```js
let a = 5;
let b = "5";
```

Teste `==` puis `===` et observe la différence.

---

## 🧠 Partie 3 – Opérateurs logiques

### Exercice 6 – Conditions composées

Crée trois variables :

```js
let a = 10, b = 20, c = 30;
```

Affiche le résultat des expressions suivantes :

- `(a < b) && (b < c)`
- `(a > b) || (b < c)`
- `!(a == b)`

---

### Exercice 7 – Combinaison pratique

Demande à l’utilisateur son âge et teste s’il est :

- majeur **et** autorisé à conduire
- mineur **ou** non autorisé à conduire  
*(tu peux simuler avec `let permis = true;`)*

---

## Partie 4 – Concaténation & Template literals

### Exercice 8 – Phrase dynamique

Demande le prénom et l’âge, puis affiche :

Bonjour Fatou, tu as 19 ans.

 Faire une fois avec `+` et une fois avec les backticks (`).

---

### Exercice 9 – Présentation

Crée trois variables : `nom`, `ville`, `pays`  
et affiche :  

```js
"Je m'appelle [nom], je vis à [ville] au [pays]."
```

---

## Partie 5 – Conversion de types

### Exercice 10 – Bug de comparaison

Demande deux nombres via `prompt()` sans conversion, puis compare-les avec `>`.  
Refais ensuite la comparaison avec `Number()` pour montrer la différence.

---

### Exercice 11 – Addition correcte

Demande deux valeurs via `prompt()` et affiche leur somme réelle (pas concaténée).

---

## Partie 6 – Booléens simples

### Exercice 12 – Test de vérité

Crée une variable `let estMajeur = true;`  
Si elle vaut `true`, affiche `"Tu peux voter."`  
Change ensuite sa valeur en `false` et observe le résultat.

---

### Exercice 13 – Expression logique

Crée deux booléens :  

```js
let a = true;
let b = false;
```

Affiche les résultats de :

- `a && b`
- `a || b`
- `!a`

---

## Partie 7 – Mini projets

### Exercice 14 – Mini calculatrice

L’utilisateur entre deux nombres et choisit une opération parmi `+`, `-`, `*`, `/`, `%`.  
Le programme affiche le résultat correspondant.

---

### Exercice 15 – Devine le bon âge

Crée une variable `ageSecret = 18`  
L’utilisateur entre un nombre avec `prompt()`  
Le programme affiche :
