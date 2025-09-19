# Nom du projet : AgentCoach

## 🎯 Contexte du projet

Un agent conversationnel sur Telegram qui permet de suivre ses performances historiques.

---

## 🛠️ Étapes du projet

1. **Télécharger** le fichier JSON `Coach AI N8N` depuis ce dépôt Git.
2. **Créer un compte** sur [N8N](https://n8n.io/).
3. **Créer et ouvrir un workspace** sur N8N, puis **importer** le fichier JSON téléchargé pour ajouter le workflow de l'agent Coach IA.
4. **Créer un bot** Telegram en suivant ce tutoriel : [Créer un bot Telegram](https://www.youtube.com/watch?v=Li2xrdRYP5o).
5. **Ajouter l'API du bot** Telegram dans la section `credentials` en cliquant sur le premier élément du workflow : `telegram trigger` + choisir dans la section `Trigger` "On Message".
6. **Choisir un modèle conversationnel** (Gemini, OpenAI, Anthropic) dans l’élément `Chat Model` du composant `AI Agent` – ici, le modèle choisi est **Gemini 2.5 Flash**.
7.  **Dans l’élément `Chat Model`** Besoin du crédential Google Gemini pour s'y connecter. En **optionnel** : 1- Modifier le sampling temperature pour avoir des réponses plus pertinentes '0.8 ou 0.9' / 2-déliminter le nombre de Maximum Token à '20048'
8. **Modifier le system message prompt** dans l’élément `AI Agent` pour adapter ton objectif et performance historique : example de prompt : 
**Role**
Tu es un coach sportif personnel specialiste dans le gain de muscle et de poid pour les personnes ayant un métabolisme ectomorphe.
**Outil**
tu as accès à mes sessions de sport historique depuis trois fichiers Get_Workout_23 , Get_Workout_24 et Get_Workout_25 dans chacun tu trouveras des données spécifiques à une année . Pour Get_Workout_23 c'est 2023 pour Get_Workout_24 c'est 2024 Get_Workout_25 c'est 2025
**Objectif**
En janvier 2025 mon poid était de 84 kilo, avec un taux de griasse corporelle à 10.9% avec un IMC à 23. Contre un poid de 83 kilo en mai 2024 avec un taux de griasse corporelle à 9.2%. Ma masse musculaire est la même depuis 2 ans c'est à dire à 43.4 kilos. Je souhaite que tu m'informes sur mes meilleurs séances , celle qui maident à muscler la partie de mon corps visé. Mais surtout que me suis en me proposant des séances plus intéréssantes pour me pousser d'avantage à progresser. Mon objectif est d'avoir un poid de corps à 88 kilo avec une masse graisseuse en dessous des 11%.
9.**Rajouter l'élement** Simple memory à ton composant Langchain 'AI AGENT' et choisir '5' comme Context Window Length (cet élément permet de récupérer les derniers messages de la conversation avec l'utilisateur et éviter que l'utilisateur se répète)
10. **Créer un ou N fichier(s) personnel(s)** Google Sheet ou Google Doc avec tes performances sportives et **le/les lier** à ton workflow.
11. **Tester le workflow** pour s’assurer qu’il fonctionne correctement.
12. **Activer le workflow** pour utiliser l’agent en production.

---

## ✅ Pré-requis

- Un **compte Google Cloud** pour créer des credentials et connecter un fichier Google Sheets ou Google Docs.
- Un **compte OpenAI ou Gemini** pour obtenir une API Key pour le modèle conversationnel.
- Un **bot Telegram** et son **token d'accès**.

---

## 🔍 Remarque

Ce projet ne nécessite **aucune connaissance en code**.
