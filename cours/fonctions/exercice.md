# Série d’exercices : Les fonctions en JavaScript

**Niveau 1 –** Bases des fonctions
*Exercice 1* : Bonjour !

Crée une fonction direBonjour() qui affiche dans la console :

"Bonjour tout le monde !"

💡 Appelle la fonction 2 fois.

*Exercice 2* : Bonjour personnalisé

Crée une fonction saluer(nom) qui affiche :

"Bonjour [nom] !"
puis appelle-la avec plusieurs prénoms.

*Exercice 3*: Addition simple

Crée une fonction addition(a, b) qui retourne la somme de a et b.
Affiche le résultat avec console.log().

*Exercice 4* : Multiplication

Crée une fonction multiplier(x, y) qui retourne le produit de deux nombres.

💬 Exemple : multiplier(3, 4) → 12

*Exercice 5* : Calcul d’âge

Crée une fonction calculerAge(anneeNaissance) qui retourne l’âge d’une personne en 2025.

**Niveau 2** – Paramètres, conditions et retour
*Exercice 6* : Pair ou impair

Crée une fonction estPair(nombre) qui affiche :

"Le nombre est pair" si c’est pair

"Le nombre est impair" sinon

*Exercice 7* : Conversion Celsius → Fahrenheit

Crée une fonction toFahrenheit(celsius) qui retourne la température en Fahrenheit.

Formule : F = (C × 9/5) + 32

*Exercice 8* : Moyenne de 3 nombres

Crée une fonction moyenne(a, b, c) qui retourne la moyenne des trois nombres.

*Exercice 9* : Calcul du carré et du cube

Crée deux fonctions :

carre(n) → retourne le carré

cube(n) → retourne le cube

Puis affiche leurs résultats pour un nombre donné.

*Exercice 10* : Salutation selon l’heure

Crée une fonction salutation(heure) :

Si heure < 12 → "Bonjour"

Si heure < 18 → "Bon après-midi"

Sinon → "Bonsoir"

**Niveau 3**– Fonctions fléchées et anonymes
*Exercice 11* : Fonction fléchée

Écris une fonction fléchée carre qui retourne le carré d’un nombre.
Teste-la avec plusieurs valeurs.

*Exercice 12* : Fonction anonyme

Crée une fonction anonyme qui retourne la somme de deux nombres, et affecte-la à une variable somme.

Appelle somme(2, 5) et affiche le résultat.

*Exercice 13* : Valeur par défaut

Crée une fonction bonjour(nom = "inconnu") qui affiche :

"Bonjour [nom] !"

*Exercice 14* : Mini calculatrice

Crée une fonction calcul(a, b, operateur) :

Si operateur = "+", additionne

Si operateur = "-", soustrait

Si operateur = "*", multiplie

Si operateur = "/", divise
Sinon affiche "Opérateur non reconnu"

**Niveau 4**– Fonctions avancées
*Exercice 15* : Callback simple

Crée une fonction faireAction(action) qui exécute une fonction passée en paramètre :

function faireAction(callback) {
  callback();
}

Appelle-la avec une fonction qui affiche "Action exécutée !"

*Exercice 16* : Somme d’un tableau

Crée une fonction sommeTableau(tab) qui retourne la somme des éléments d’un tableau numérique.

Exemple : [2, 5, 3] → 10

*Exercice 17* : Plus grand nombre

Crée une fonction max(a, b, c) qui retourne le plus grand des trois nombres.

*Exercice 18* : Compter les voyelles

Crée une fonction compterVoyelles(texte) qui compte le nombre de voyelles (a, e, i, o, u, y) dans une chaîne.

Exemple : "javascript" → 3

*Exercice 19* : Fonction imbriquée

Crée une fonction parent() qui contient une fonction enfant().
enfant() doit afficher "Coucou depuis l’enfant", et parent() doit l’appeler.

*Exercice 20* : Générateur de mot de passe

Crée une fonction genererMotDePasse(longueur) qui retourne une chaîne aléatoire de lettres et chiffres.

Exemple : genererMotDePasse(6) → "a9b2xk"

🏆 Challenge final
✨ Exercice 21 : Mini programme

Crée une fonction calculerSalaire(nom, heures, tauxHoraire) qui :

Calcule le salaire brut (heures * tauxHoraire)

Si heures > 40, applique une prime de 10%

Affiche :

"[nom] a gagné [montant] FCFA cette semaine."
Appelle la fonction avec différents employés.
