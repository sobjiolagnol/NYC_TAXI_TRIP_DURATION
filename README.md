

---

```markdown
# NYC_TAXI_TRIP_DURATION

Projet de data science et de machine learning visant à **analyser et prédire la durée des trajets en taxi à New York City**, à partir de données historiques fournies par la NYC Taxi and Limousine Commission (TLC).  
Ce dépôt contient le code pour le **prétraitement des données**, l'**entraînement de modèles de prédiction**, l'**exposition d'une API**, ainsi que des **outils d'évaluation**.

---

## Contexte

Les célèbres taxis jaunes de New York – au nombre de 12 779 – desservent environ 240 millions de passagers chaque année, générant une industrie de 1,8 milliard de dollars.  
Comprendre et prédire la durée des trajets en taxi peut fournir des informations précieuses aux urbanistes, aux citoyens et aux acteurs du transport.

Ce projet s’appuie sur les données de la compétition Kaggle ["New York City Taxi Trip Duration"](https://www.kaggle.com/competitions/nyc-taxi-trip-duration), qui met à disposition les enregistrements de trajets de 2016.  
L’objectif est de construire un **modèle multivarié capable de prédire la durée totale d’un trajet** en fonction de divers facteurs comme l’heure, la distance, les coordonnées géographiques, etc.

---

## Structure du projet

```

.
├── API.py               # API FastAPI ou Flask pour l'exposition du modèle
├── common.py            # Fonctions utilitaires partagées
├── config.ini           # Configuration globale du projet
├── evaluate.py          # Script d’évaluation des performances du modèle
├── main.py              # Script principal de lancement ou de tests
├── train.py             # Entraînement du modèle
├── requirements.txt     # Dépendances Python
├── README.md            # Ce fichier


````

---

## Prérequis

- Python 3.x installé et accessible depuis la ligne de commande.
- Installer les dépendances avec :

```bash
pip install -r requirements.txt
````

---

## Utilisation

### 1. Entraîner le modèle :

```bash
python train.py
```

### 2. Lancer l’API (ex: avec FastAPI) :

```bash
uvicorn API:app --reload
```

Puis ouvrir dans un navigateur :
[http://127.0.0.1:8000](http://127.0.0.1:8000)

### 3. Évaluer le modèle :

```bash
python evaluate.py
```


