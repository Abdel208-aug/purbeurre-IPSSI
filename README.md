# PurBeurre - IPSSI

## Description

PurBeurre - IPSSI est une application web développée avec Django qui utilise une base de données MySQL. Elle interagit avec l'API d'Open Food Facts pour récupérer des informations sur les aliments, les comparer, et proposer des substituts plus sains ou non allergènes.

## Fonctionnalités

- Récupération des données alimentaires via l'API d'Open Food Facts.
- Comparaison des aliments en termes de santé et d'allergènes.
- Proposition de substituts alimentaires plus sains ou non allergènes.
- Interface utilisateur intuitive pour rechercher et visualiser les informations sur les aliments.

## Prérequis

- Python 3.x
- Django 3.x ou supérieur
- MySQL
- Pipenv (optionnel, mais recommandé pour la gestion des dépendances)

## Installation

### 1. Cloner le dépôt

```bash
git clone https://github.com/Abdel208-aug/purbeurre-IPSSI.git
cd purbeurre-IPSSI
```

#### 2. Installer les dépendances
Utiliser Pipenv pour créer un environnement virtuel et installer les dépendances :
```bash
pipenv install
pipenv shell
```
### 3. Configurer la base de données MySQL
Créer une base de données MySQL et mettre à jour settings.py avec vos informations de connexion MySQL :

```bash
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'nom_de_votre_base_de_donnees',
        'USER': 'votre_utilisateur',
        'PASSWORD': 'votre_mot_de_passe',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```
### 4. Migrer la base de données
```bash
python manage.py runserver
```
### 5. Lancer le serveur de développement

```bash
python manage.py runserver
```
## Utilisation
### 1. Accéder à l'application
Ouvrez votre navigateur et accédez à http://127.0.0.1:8000.

### 2. Rechercher des aliments
Utilisez la barre de recherche pour entrer le nom d'un aliment et obtenir des informations détaillées.

### 3. Voir les substituts proposés
Sur la page des détails de l'aliment, vous trouverez une liste de substituts plus sains ou non allergènes.
