# Demo 01 - Introduction à Git
Ceci est un projet de démo de l'utilisation de git !

## Les commandes de base

### Initialize la gestion avec GIT
```
git init
```

### Configurer les données de l'utilisateur
```
git config user.name "<nom de l'utilisation>"
git config user.email "<email de l'utilisation>"

NB : Ajouter « --global » pour réaliser une config global sur la machine.
```

### Verifier l'etat de git
```
git status
```

### Obtenir la liste des commit
```
git log --oneline
```

### Sauvegarder le fichiers → Les versionner avec git
```
# Ajouter les fichiers à valider (Stage)
git add <fichier>
git add <dossier>
git add .

# Valider les fichiers selectionnée (Commit)
git commit -m "<message>"
```

## Le fichier ".gitignore"
Son objectif est d'éviter d'envoyer dans git : 
- Des informations sensibles _(Par exemple, le fichier d'env avec des mdp)_
- Des fichiers ou dossiers inutiles _(Cache, Config local, Dépendence, ...)_

[Dépot github avec des templates de gitignore](https://github.com/github/gitignore)


## Interaction avec le depot distant

### Liste non exaustive
- Github
- GitLab
- Azuze DevOps
- Bitbucket
- ...

### Commande
- Projet créer en local qu'on lie avec le repo distant
```
# Création du lien
git remote add origin https://github.com/FormCours/TF_2026_DataAnalyst_Indus__Git_Demo

# Envoyer des données vers le repo
# - Avec la relation (Nom de la remote et le nom de branche sur le repo)
git push origin main

# - Avec la relation configuré (Idem sauf que la config sauvegarder)
git push -u origin main

# - Si la relation est configuré
git push
```

- Récuperation d'un projet distant
```
# Clone du repo (Le lien entre l'origin et le local est configuré)
git clone <url-repo>

# Clone d'un repo en nommant le dossier
git clone <url-repo> <nom>
```

- Travaillé avec un repo distant
```
# Envoyer les commits
git push

# Récuperer les commits sans les appliquer
git fetch

# Récuperer et appliquer les commits
git pull
```