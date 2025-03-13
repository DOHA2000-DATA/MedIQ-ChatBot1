# MedIQ-ChatBot1


![249312156-423d76c6-98fd-4365-8fee-a55f45fd6cd6](https://github.com/user-attachments/assets/6a3dc27d-69d0-422f-a691-ada72506fc57)


## 📌 Description
MedIQ-ChatBot est un chatbot basé sur Flask, conçu pour répondre à des questions médicales en utilisant des intentions définies dans un fichier JSON. Il est développé avec **LSTM (Long Short-Term Memory), un type de RNN (Recurrent Neural Network)**, en utilisant **Keras et TensorFlow** pour l'entraînement et la gestion des modèles d'intelligence artificielle. Il est déployable avec Docker et intègre des pipelines CI/CD via GitHub Actions.

## 🚀 Fonctionnalités
- Répond aux questions basées sur des intentions pré-entraînées avec un modèle de deep learning (LSTM RNN)
- Utilise **TensorFlow et Keras** pour entraîner le modèle et effectuer des prédictions
- Utilise Flask pour gérer les requêtes HTTP
- Déployable avec Docker et Docker Compose
- Intègre des workflows CI/CD pour automatiser le déploiement

## 🛠️ Installation et Exécution

### Prérequis
- Python 3.x
- pip
- Docker (optionnel pour le déploiement via conteneur)

### Installation
1. **Cloner le dépôt**
   ```bash
   git clone https://github.com/VOTRE_NOM_UTILISATEUR/NOM_DU_REPO.git
   cd NOM_DU_REPO
   ```
2. **Créer un environnement virtuel (optionnel mais recommandé)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Sur Windows : venv\Scripts\activate
   ```
3. **Installer les dépendances**
   ```bash
   pip install -r flask/requirements.txt
   ```

### Entraînement du modèle
Si vous souhaitez réentraîner le modèle avec de nouvelles données, exécutez :
```bash
python flask/train.py
```
Cela entraînera le modèle en utilisant **TensorFlow/Keras et LSTM** et générera un fichier modèle enregistré.

### Exécution du chatbot

#### 📍 Méthode 1 : Lancer avec Flask
```bash
python flask/main.py
```
Accéder ensuite à l'application via [http://127.0.0.1:5000](http://127.0.0.1:5000).

#### 📍 Méthode 2 : Lancer avec Docker
```bash
docker-compose up --build
```

## 📂 Structure du projet
```
MedIQ-ChatBot/
│── flask/
│   │── main.py             # Fichier principal du serveur Flask
│   │── intents.json        # Définitions des intentions du chatbot
│   │── train.py            # Script d'entraînement du modèle LSTM
│   │── model.h5            # Modèle entraîné avec Keras
│   │── requirements.txt    # Dépendances Python
│   │── Dockerfile          # Fichier pour créer l'image Docker
│── .github/workflows/      # Workflows CI/CD
│── docker-compose.yml      # Déploiement multi-conteneurs
│── README.md               # Documentation du projet
```

## 📜 License
Ce projet est sous licence MIT. Vous êtes libre de l'utiliser, le modifier et le partager.

## 🤝 Contribuer
Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une **issue** ou une **pull request**.

---
🚀 **Développé avec passion en utilisant LSTM, Keras et TensorFlow !**

# MERCI POUR VOTRE ATTENTION
