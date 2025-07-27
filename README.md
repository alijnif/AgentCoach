# Nom du projet : AgentCoach
**Contexte du projet** Un Agent conversationnel sur telegram qui permet de suivre ses performances historiques

**Etapes du projet**
1 - Telecharger le fichier JSON "Coach AI N8N" dans ce Git 
2 - Ouvrir et creer un compte N8N 
3 - Créer et ouvrir un workspace (espace de travail) sur N8N et importer le fichier JSON telechargé pour rajouter le workflow de l'agent Coach IA
4 - Créer un bot sur telegram en suivant ce lien https://www.youtube.com/watch?v=Li2xrdRYP5o
5 - Rajouter l'API du bot généré de telegram dans "credential to connect with" en cliquant sur le premier element du workflow "telegram trigger"
6 - Rajouter son modèle conversationnel (Gemini, OPENAI, Anthropic) dans l'element "Chat Model" du composant "AI Agent", ici le modèle choisi est Gemini 2.5 flash
7 - Changer le System Message prompt en cliquant sur l'element "AI Agent" pour modifier ton objectif et performance historique 
8 - Creer un un fichier personnel sur GoogleSheet ou GoogleDoc avec ses performances historiques de sport et les liers
9 - Tester le workflow pour s'assurer qu'il fonctionne bien 
10 - Activer le workflow pour utiliser l'agent en production

**Pre-requis**
1 - Compte Google cloud pour la création de credentials et liaison d'un fichier GoogleSheets ou GoogleDoc
2 - Compte OPENAI ou GEMINI pour recevoir une API KEY pour lier le modele conversationnel
3 - BOT Telegram et son numéro de token  

Projet n'a pas besoin de connaissance en code
