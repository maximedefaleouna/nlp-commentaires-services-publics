# Classification de commentaires citoyens

Projet de traitement automatique du langage naturel (NLP) visant à classifier des commentaires citoyens sur les services publics en trois catégories : **Satisfaction**, **Insatisfaction** et **Suggestion**.

Le notebook explore le jeu de données, prépare les textes, les représente avec TF-IDF, entraîne et compare des modèles de classification, puis analyse leurs résultats et leurs erreurs. Les commentaires sont principalement en français, avec quelques termes en éwé/mina.

## Fichiers

- `DEFALEOUNA_Tchassama_Dessoklema(nlp_test).ipynb` : analyse et entraînement des modèles.
- `dataset_nlp_test_tal.csv` : jeu de données utilisé par le notebook.
- `requirements.txt` : dépendances Python.

## Prérequis

- Python 3.9 ou plus récent
- `pip`

## Installation

Depuis le dossier du projet, créez puis activez un environnement virtuel :

```bash
python -m venv .venv
source .venv/bin/activate
```

Sous Windows, activez-le avec :

```powershell
.venv\Scripts\Activate.ps1
```

Installez les dépendances :

```bash
python -m pip install -r requirements.txt
```

## Lancement

Démarrez Jupyter depuis la racine du projet :

```bash
jupyter notebook
```

Ouvrez ensuite `DEFALEOUNA_Tchassama_Dessoklema(nlp_test).ipynb` et exécutez les cellules dans l'ordre. Le fichier `dataset_nlp_test_tal.csv` doit rester dans le même dossier que le notebook. Le notebook télécharge les stopwords français de NLTK lors de son exécution ; une connexion Internet peut être nécessaire si cette ressource n'est pas déjà installée.