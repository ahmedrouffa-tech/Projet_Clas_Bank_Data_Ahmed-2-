# 🏦 Prédiction de Souscription au Dépôt à Terme

Ce projet contient une application web interactive construite avec **Streamlit** et propulsée par un modèle **XGBoost** optimisé. L'objectif est de prédire si un client souscrira à un dépôt à terme à l'issue d'une campagne de marketing direct.

## 📂 Structure du Projet

- `app.py` : Le code source de l'interface utilisateur Streamlit.
- `list_items.joblib` : Fichier de configuration contenant le modèle XGBoost entraîné, le normaliseur (scaler) et les valeurs uniques pour les formulaires.
- `requirements.txt` : Liste des dépendances Python requises pour exécuter l'application.

## 🚀 Installation et Lancement Local

### 1. Cloner le dépôt
```bash
git clone <URL_DE_VOTRE_DEPOT_GITHUB>
cd <NOM_DU_DOSSIER>
```

### 2. Installer les dépendances
Il est recommandé d'utiliser un environnement virtuel :
```bash
pip install -r requirements.txt
```

### 3. Lancer l'application Streamlit
```bash
streamlit run app.py
```

## 📊 Caractéristiques du Modèle
- **Modèle sélectionné** : XGBoost Classifier
- **Score d'exactitude (Accuracy)** : ~87% sur l'ensemble de test
- **Variables clés** : Durée de l'appel (`duration`), âge (`age`), résultat de la campagne précédente (`poutcome`).
