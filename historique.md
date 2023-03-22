# Historique des commandes du TP1

### Création d'un dépot

> - Initialise un dépot vide, cette commande est éxécuté une seule fois
> - Si on l'éxécute une deuxiéme fois on détruit le dépot 
- `git init`

---
### Vérifier le status
- `git status`
---
### Afficher l'historique des commits
- `git log`
- `git log --oneline`
---
### Naviguer dans les branches
- Pour changer le nom d'une branche
  - `git branch -m <<nom nouvelle branche>>`
  - `git branch -m main`
- Pour créer une nouvelle branche
  - `git branch <<nouvelle branche>>`
- Pour changer de branche
  - `git checkout << la branche>>`
  - On ne peut pas changer de branche si la branche courante n'a pas été <<commit>> valider
  - `git checkout << id du commit >>`
  - `git checkout << étiquette du commit >>`
- Pour créer une étiquette 
  - `git tag v1.0.0 // Création de l'étiquette v1.0.0`
  - `git tag // permet d'afficher l'ensemble des tag (étiqutte)` 
  - `git checkout v1.0.0 // pour se déplacer dans le commit v1.0.0 (déplace le pointeur <<head>>)`
---
### Serveur distant
- Pour définir un alias identifiant le serveur distant
  - `git remote add 41e https://github.com/dorahim87/41e.git`
  - `git remote -v`// voir la liste des alias du serveur distant
  - `git push 41e main` // pousser mon dernier commit vers la branche main du dépot distant 41e
