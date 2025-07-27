# Nom du projet : AgentCoach

## 🎯 Contexte du projet

Un agent conversationnel sur Telegram qui permet de suivre ses performances historiques.

---

## 🛠️ Étapes du projet

1. **Télécharger** le fichier JSON `Coach AI N8N` depuis ce dépôt Git.
2. **Créer un compte** sur [N8N](https://n8n.io/).
3. **Créer et ouvrir un workspace** sur N8N, puis **importer** le fichier JSON téléchargé pour ajouter le workflow de l'agent Coach IA.
4. **Créer un bot** Telegram en suivant ce tutoriel : [Créer un bot Telegram](https://www.youtube.com/watch?v=Li2xrdRYP5o).
5. **Ajouter l'API du bot** Telegram dans la section `credentials` en cliquant sur le premier élément du workflow : `telegram trigger`.
6. **Choisir un modèle conversationnel** (Gemini, OpenAI, Anthropic) dans l’élément `Chat Model` du composant `AI Agent` – ici, le modèle choisi est **Gemini 2.5 Flash**.
7. **Modifier le system message prompt** dans l’élément `AI Agent` pour adapter ton objectif et performance historique.
8. **Créer un fichier personnel** Google Sheet ou Google Doc avec tes performances sportives et **le lier** à ton workflow.
9. **Tester le workflow** pour s’assurer qu’il fonctionne correctement.
10. **Activer le workflow** pour utiliser l’agent en production.

---

## ✅ Pré-requis

- Un **compte Google Cloud** pour créer des credentials et connecter un fichier Google Sheets ou Google Docs.
- Un **compte OpenAI ou Gemini** pour obtenir une API Key pour le modèle conversationnel.
- Un **bot Telegram** et son **token d'accès**.

---

## 🔍 Remarque

Ce projet ne nécessite **aucune connaissance en code**.
