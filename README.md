🎓 BrainMovie – Système de Recommandation de Films

Ce projet a été réalisé dans le cadre d’un projet académique.
Il consiste à concevoir et implémenter un système intelligent de recommandation de films basé sur le Content-Based Filtering.

📌 Contexte académique
Type : Projet académique
Auteur : Brahim Benrais
Domaine : Data Science / Machine Learning
🎯 Objectifs
Analyser les caractéristiques des films
Construire un système de recommandation basé sur le contenu
Générer des recommandations personnalisées
Évaluer la pertinence des résultats
🧠 Méthodologie
Exploration et nettoyage des données
Transformation des données textuelles
Vectorisation avec TF-IDF
Calcul de similarité avec Cosine Similarity
Génération de recommandations (Top-N)
📊 Dataset

Le projet utilise le dataset MovieLens, contenant :

Titres des films
Genres
Descriptions
Évaluations des utilisateurs
🛠️ Technologies utilisées
Python
Pandas
Scikit-learn
TfidfVectorizer
Cosine Similarity (linear_kernel)
Streamlit
Docker
⚙️ Fonctionnement

Lorsqu’un utilisateur sélectionne un film :

Le système identifie le film dans la base de données
Analyse ses caractéristiques
Calcule la similarité avec les autres films
Sélectionne les films les plus proches
Affiche les recommandations
📈 Résultats

Le système permet de proposer des recommandations pertinentes et rapides basées sur les caractéristiques des films.

🚀 Déploiement

L’application est conteneurisée avec Docker, ce qui facilite :

L’installation
La portabilité
Le déploiement
🔮 Perspectives
Intégration du filtrage collaboratif
Mise en place d’un système hybride
Utilisation du Deep Learning
📌 Conclusion

BrainMovie démontre l’efficacité des techniques de Machine Learning dans les systèmes de recommandation.
L’approche basée sur TF-IDF et la similarité cosinus permet de générer des recommandations adaptées aux préférences des utilisateurs.
