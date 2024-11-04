# Tp1_Git

- Comment vérifier la configuration actuelle de Git sur votre machine, notamment le nom d’utilisateur et l’adresse e-mail ?

```bash
git config --list
```

- Comment modifier votre adresse e-mail si vous l'avez mal configurée lors de l'installation de Git ?

```bash
git config --global user.email "new_email@example.com"
```

- Si vous avez oublié de créer un fichier README.md lors de l'initialisation du projet, comment pouvez-vous l'ajouter après coup et commiter les changements ?

```bash
git add README.md
git commit -m "Add README.md"
```

- Comment définir un dépôt distant si vous n'en avez pas configuré un lors de la création du projet ?

```bash
git remote add origin <remote_repository_url>
git push -u origin main
```

- Comment annuler les modifications locales d'un fichier avant de les ajouter à l'index ?

```bash
git checkout -- <filename>
```

- Comment visualiser les fichiers qui sont prêts à être commités dans Git (staging) ?

```bash
git status
```

- Comment suivre (track) un dépôt distant et récupérer toutes les branches de ce dépôt ?

```bash
git remote add origin <remote_repository_url>
git fetch --all
git branch --track <local_branch_name> <remote_branch_name>
```

- Comment supprimer une branche locale après l'avoir fusionnée dans master ?

```bash
git branch -d <branch_name>
```

- Comment interrompre un rebase en cours si vous avez commis une erreur ?

```bash
git rebase --abort
```

- Comment lister les commits qui vont être rebasés avant de lancer un rebase ?

```bash
git rebase --onto <new_base> <old_base>
```

- Comment afficher la liste des branches actives et en cours de développement dans Gitflow ?

```bash
git branch
```

- Comment annuler une branche de correctif (hotfix) avant de la finaliser si vous constatez
une erreur ?

```bash
git checkout develop
git branch -D hotfix/<hotfix_name>
```
