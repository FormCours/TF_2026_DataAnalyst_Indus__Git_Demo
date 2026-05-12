# Demo GIT 01
Ceci est un projet de démo de l'utilisation de git !

## Les commandes de base 
Initialize la gestion avec GIT
```
git init
```

Configurer les données de l'utilisateur
```
git config user.name "<nom de l'utilisation>"
git config user.email "<email de l'utilisation>"

NB : Ajouter « --global » pour réaliser une config global sur la machine.
```

Sauvegarder le fichiers → Les versionner avec git
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

Dépot github avec des templates de gitignore :  
https://github.com/github/gitignore