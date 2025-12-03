# Projet : Analyse des Sentiments et Détection des Tendances

## Description
Ce projet vise à analyser les sentiments d’un texte et détecter les tendances à partir de données textuelles. Il fournit un tableau de bord interactif pour visualiser les résultats et inclut des fonctionnalités d’authentification via une page de login et d’inscription.  

Le projet utilise un modèle de langage avancé (LLM) et **DistilBERT** pour l’analyse des sentiments et des tendances.

## Technologies Utilisées
- **Frontend** : React, Tailwind CSS (ou autre framework CSS pour stylisation)
- **Backend** : FastAPI
- **Base de données** : Supabase (PostgreSQL)
- **Modèles NLP** : DistilBERT, modèles LLM pour analyse avancée
- **Méthodologie** : CRISP-DM (Cross Industry Standard Process for Data Mining)

## Fonctionnalités
1. **Analyse de sentiments** : Détermination du sentiment global (positif, négatif, neutre) pour un texte donné.
2. **Détection des tendances** : Identification des sujets ou mots-clés les plus fréquents dans un ensemble de textes.
3. **Tableau de bord** : Visualisation interactive des résultats (graphes, nuages de mots, histogrammes).
4. **Authentification utilisateur** :
   - Page de login
   - Page d’inscription
   - Gestion sécurisée des sessions
5. **Historique et suivi** : Possibilité pour les utilisateurs de consulter les analyses précédentes.

## Architecture

## Méthodologie CRISP-DM
1. **Compréhension du business** : Identifier le besoin d’analyse des sentiments et tendances pour les textes.
2. **Compréhension des données** : Collecte des textes à analyser.
3. **Préparation des données** : Nettoyage, tokenization et vectorisation des textes.
4. **Modélisation** : Utilisation de DistilBERT et LLM pour l’analyse des sentiments et détection des tendances.
5. **Évaluation** : Vérification de la précision et de la pertinence des résultats.
6. **Déploiement** : Mise en place de l’application web avec dashboard interactif et gestion des utilisateurs.

## Installation et Déploiement

### Prérequis
- Node.js et npm
- Python 3.11+
- Supabase CLI
- Git

### Backend
```bash
cd backend
python -m venv venv
source venv/bin/activate  # sur Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
cd frontend
npm install
npm start
Configuration Supabase

Créer un projet Supabase

Configurer la base de données et récupérer les clés API

Ajouter les variables d’environnement dans .env.local :
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
/frontend    -> React app
/backend     -> FastAPI backend
/models      -> Modèles NLP (DistilBERT / LLM)
/utils       -> Scripts utilitaires pour preprocessing et visualisation
