# 🧭 GIT – Les commandes essentielles pour débuter

Ce document regroupe les **commandes Git de base** pour gérer ton projet et apprendre à collaborer via GitHub.

---

## ⚙️ 1. Initialiser un projet Git
Créer un dépôt Git local dans un dossier (si ce n’est pas déjà fait) :
```bash
git init
```
> Cela crée un dossier caché `.git` qui contient tout l’historique du projet.

---

## 📂 2. Vérifier le statut du projet
Voir les fichiers modifiés, nouveaux ou supprimés :
```bash
git status
```

---

## ➕ 3. Ajouter des fichiers au suivi
Avant d’enregistrer des changements, il faut les “stager” :
```bash
git add fichier.js
```
ou pour tout le dossier :
```bash
git add .
```

---

## 💾 4. Enregistrer les changements
Créer un **point de sauvegarde** avec un message clair :
```bash
git commit -m "Ajout des exercices sur les conditions"
```

---

## 🔍 5. Voir l’historique des commits
Afficher tous les commits faits :
```bash
git log
```
👉 Astuce rapide :
```bash
git log --oneline
```

---

## 🌐 6. Lier ton dossier à GitHub (une seule fois)
Après avoir créé ton dépôt vide sur GitHub :

```bash
git remote add origin https://github.com/ton_compte/nom_du_depot.git
```

Vérifie la connexion :
```bash
git remote -v
```

---

## 🚀 7. Envoyer ton travail vers GitHub
Pousser ton code en ligne :
```bash
git push -u origin main
```
(premier push)  
Ensuite, simplement :
```bash
git push
```

---

## ⬇️ 8. Récupérer les nouvelles mises à jour
Quand toi ou un camarade modifie le dépôt :
```bash
git pull
```

---

## 🔄 9. Mettre à jour ton dépôt local
Si tu veux **fusionner les nouveautés** en local :
```bash
git fetch
git merge
```
> (Souvent `git pull` suffit, car il fait les deux.)

---

## 🌿 10. Gérer les branches

### Créer une nouvelle branche
```bash
git branch nom_de_branche
```

### Se déplacer vers une autre branche
```bash
git checkout nom_de_branche
```

### Créer et aller directement sur une branche
```bash
git checkout -b nom_de_branche
```

### Fusionner une branche avec la branche principale
Une fois le travail terminé sur ta branche :
```bash
git checkout main
git merge nom_de_branche
```
> ⚠️ Fais toujours un `git pull` avant de fusionner pour éviter les conflits.

### Supprimer une branche après fusion
```bash
git branch -d nom_de_branche
```

---

## ✏️ 11. Modifier un fichier et changer de branche

Si tu as modifié un fichier mais que tu veux **changer de branche**, tu dois d’abord :
1. Soit **enregistrer ton travail** :
   ```bash
   git add .
   git commit -m "Sauvegarde temporaire avant de changer de branche"
   ```
2. Soit **le mettre de côté temporairement** :
   ```bash
   git stash
   git checkout autre_branche
   ```
   Et quand tu veux récupérer ton travail :
   ```bash
   git stash pop
   ```

---

## 🚫 12. Ignorer certains fichiers
Créer un fichier `.gitignore` et y mettre :
```
node_modules/
.DS_Store
.env
```
> Tout ce qui ne doit **pas être poussé** sur GitHub.

---

## 🧹 13. Quelques commandes utiles

### Voir la différence entre fichiers
```bash
git diff
```

### Supprimer un fichier du suivi (sans le supprimer du dossier)
```bash
git rm --cached fichier.js
```

### Changer le message du dernier commit
```bash
git commit --amend -m "Nouveau message plus clair"
```

---

## 💡 Routine quotidienne conseillée

1. `git pull` → pour avoir la dernière version  
2. Faire les modifications ou exercices  
3. `git add .` → ajouter tous les fichiers  
4. `git commit -m "Description du travail fait"`  
5. `git push` → envoyer sur GitHub  

---

🧠 *Astuce : plus tu pratiques ces commandes, plus elles deviendront naturelles.*
