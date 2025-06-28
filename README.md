JURIBOT RDC

Assistant juridique intelligent spécialisé dans le droit congolais

Description
----------

JURIBOT est une application intelligente conçue pour aider les citoyens congolais, particuliers ou entreprises, à obtenir des explications claires et vulgarisées sur des questions juridiques en lien avec la loi congolaise dans certains domaines. L'outil repose sur des techniques modernes de traitement du langage naturel (NLP) et d'intelligence artificielle.


Objectifs
---------

Créer un assistant intelligent juridique capable de comprendre le langage naturel.

Offrir un accès rapide aux articles de loi pertinents via une interface conviviale.

Permettre l'analyse de documents juridiques (PDF) et leur interprétation.

Vulgariser des notions juridiques complexes pour les rendre compréhensibles à tous.


Domaines juridiques ciblés
-------------------------

Droit du travail (contrats, licenciements, sécurité sociale, etc.)

Droit foncier (propriétés, parcelles, titres fonciers, etc.)

Droit civil et familial (succession, mariage, divorce, etc.)

Droit pénal de base (infractions courantes, dépôt de plainte, etc.)


Public cible
------------

Particuliers

Petites et moyennes entreprises

Juristes ou étudiants en droit


Fonctionnalités prévues
-----------------------

Interface de type chatbot avec moteur NLP

Lecture de documents PDF (contrats, lois, etc.)

Analyse, nettoyage, et vectorisation de textes juridiques

Réponses contextualisées selon le profil (particulier / entreprise)

Accès local via navigateur web (une possibilité d'une version mobile )


Technologies et concepts utilisés
---------------------------------

Langage : Python 3.11+

Interface : Streamlit (pour une interface web rapide et simple)

Traitement de texte : Pandas, PyMuPDF, regex

Vectorisation : FAISS (Facebook AI Similarity Search)

Moteur NLP : Google Gemini API (ou un modèle open-source alternatif)

Gestion des documents : PDF → texte nettoyé → vecteurs sémantique

Stockage local de vecteurs : vector_db/


Structure du projet
------------------

juribot_rdc/
|
|├️ juribot_app.py               # Application principale Streamlit
|├️ requirements.txt            # Modules Python requis
|├️ README.md                   # Présentation du projet
|
|├️ assets/                    # Images, logos, icônes
|├️ data/
|   ├️ documents_pdf/           # PDF des lois et codes congolais
|   └️ cleaned_texts/           # Fichiers textes nettoyés extraits des PDF
|├️ modules/
|   ├️ pdf_reader.py           # Extraction et nettoyage de PDF
|   ├️ text_splitter.py        # Division des textes en chunks
|   ├️ vector_store.py         # Stockage et recherche vectorielle FAISS
|   └️ nlp_engine.py           # Appels à l'API Gemini (ou modèle local)
|└️ vector_db/                # Base de données vectorielle locale



