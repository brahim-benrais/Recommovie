🎥 BrainMovie : Ingénierie d'un Système de Recommandation Intelligent
Projet de Spécialisation en Intelligence Artificielle & Big Data

📝 Introduction Technique
Dans le cadre de mon cursus en Intelligence Artificielle, j'ai conçu BrainMovie, une solution logicielle capable de modéliser les préférences cinématographiques. Ce projet explore la proximité sémantique entre les œuvres pour offrir des recommandations d'une grande précision, en transformant des métadonnées textuelles non structurées en vecteurs mathématiques exploitables.

🏗️ Architecture du Projet et Logique Modulaire
Pour garantir que ce projet soit Production-Ready, j'ai adopté une architecture modulaire. Chaque composant est isolé pour permettre une maintenance aisée et une scalabilité future.

1. Pipeline de Traitement des Données
Ingestion : Chargement du dataset MovieLens (Métadonnées, Titres, Résumés).

Nettoyage (Preprocessing) : Suppression des caractères spéciaux, élimination des "Stop-words" et normalisation textuelle.

Vectorisation : Transformation du texte en une matrice numérique via l'algorithme TF-IDF.

2. Flux de Travail Visuel
Extrait de code
graph TD
    subgraph "Phase de Préparation"
    A[Dataset MovieLens] --> B[Nettoyage & Normalisation]
    B --> C[Fusion des Métadonnées - Soupe de Tags]
    end

    subgraph "Phase d'Intelligence"
    C --> D[Vectorisation TF-IDF]
    D --> E[Calcul de la Matrice de Similarité]
    end

    subgraph "Phase de Delivery"
    E --> F[API Streamlit Interactive]
    F --> G[Utilisateur Final]
    end

    style C fill:#f1f1f1,stroke:#333
    style E fill:#e1f5fe,stroke:#01579b
🧠 Méthodologie et Choix Algorithmiques
L'Algorithme TF-IDF
J'ai implémenté le Term Frequency-Inverse Document Frequency pour pondérer l'importance des termes. Un mot rare mais spécifique à un genre (ex: "Espace" pour la SF) aura un poids bien plus important qu'un mot générique (ex: "Histoire"), ce qui affine la pertinence du résultat.

Pourquoi le Filtrage Basé sur le Contenu ?
Cette approche permet de résoudre le problème du "Cold Start". Le système peut recommander un film dès son ajout dans la base de données, sans attendre les évaluations des utilisateurs, simplement en analysant ses caractéristiques intrinsèques.

📂 Organisation des Ressources (Clean Architecture)
src/ : Cœur du moteur (Scripts de calcul, API Streamlit).

data/ : Répertoire dédié aux fichiers CSV optimisés.

notebooks/ : Recherches exploratoires et visualisations.

deployment/ : Fichiers de configuration Docker.

requirements.txt : Gestion des dépendances.

🛠️ Stack Technique
Langage : Python 3.x (Pandas, NumPy)

Machine Learning : Scikit-Learn

Interface : Streamlit

Conteneurisation : Docker

🚀 Guide de Mise en Œuvre Rapide
Bash
# Installation des dépendances
pip install -r requirements.txt

# Lancement via Docker
docker build -t brainmovie-app .
docker run -p 8501:8501 brainmovie-app
📈 Roadmap & Perspectives
[ ] Optimisation : Intégration de la bibliothèque FAISS pour gérer des millions de vecteurs.

[ ] Modèle Hybride : Couplage avec du Deep Learning.

[ ] CI/CD : Automatisation du déploiement via GitHub Actions.

📬 Contact & Support
Si vous avez des questions techniques ou des opportunités de collaboration, n'hésitez pas à me contacter :

Nom : Brahim Benrais

Profil : Étudiant en Développement de l'Intelligence Artificielle

Email : brahimbenrais777@gmail.com

Location : Casablanca, Maroc

Dernière mise à jour : Avril 2026 | Licence MIT
