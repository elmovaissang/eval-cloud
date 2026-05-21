# Rapport de déploiement - ARIK Zehra

## Liens
- **Application en ligne :** https://eval-cloud-elmvss.osc-fr1.scalingo.io/
- **Dépôt de code :** https://github.com/elmovaissang/eval-cloud.git

## Prérequis techniques
    - PHP 8.5 (ou 7.4)
    - Composer
    - Compte GitHub
    - Compte Scalingo

## Fichier de configuration CI
Le fichier de configuration de l'intégration continue se trouve dans :
.github/workflows/ci.yaml

## Procédure de déploiement pas à pas

A. Initialisation sur Scalingo
    1. Créer l'application

B. Ajout de variables d'environnement
Ajouter des variables d'environnement sur Scalingo
    1. APP_ENV = prod
    2. APP_SECRET = (par exemple copier la valeur de : echo bin2hex(random_bytes(16)))

C. Mise en ligne
    1. Push des commits : git push
