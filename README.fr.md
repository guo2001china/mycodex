# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)


Codex + Hermes, à la portée de tous : moins de friction autour des tokens, plus de configuration qui part en vrille, et enfin un workflow bureau qui tient la route.

MyCodex transforme Codex + Hermes en véritable espace de travail desktop. Vous ouvrez l'application, vous décrivez ce que vous voulez faire, et l'Agent prend le relais — il exécute la tâche, vous montre sa progression en direct et garde les fichiers produits à portée de main. Et si vous utilisez WeChat, vous pouvez envoyer vos tâches et récupérer vos fichiers directement depuis votre téléphone.

## v0.6.1

- Les connexions à l'authentification cloud disposent désormais d'un timeout explicite et d'une reconnexion automatique en cas de coupure réseau.
- Les paquets desktop embarquent directement l'adresse MyCodex de production, ce qui évite les échecs au premier lancement dus à des valeurs de développement local.
- Des améliorations de stabilité Windows sont incluses dans cette version : la structure zip, l'emplacement du runtime et la configuration du paquet sont désormais vérifiés avant l'ajout d'un asset Windows.
- Les paquets macOS Apple Silicon et Intel ont été reconstruits en 0.6.1.
- WeChat et Hermes restent au cœur du workflow : envoi de tâches, poursuite d'une conversation, récupération des fichiers de résultats.
- Les résultats vont bien au-delà d'une simple réponse : le déroulé, la conclusion, les tableaux, les fichiers et les prochaines étapes sont tous accessibles au sein de la même conversation.

## Le problème

Beaucoup de gens voudraient utiliser Codex + Hermes, mais abandonnent avant d'avoir accompli leur première tâche concrète — bloqués par les tokens, le terminal, le routage de modèles ou les variables d'environnement.

MyCodex ramène le démarrage à trois étapes : télécharger, se connecter, décrire sa tâche. Les résultats, le déroulé et les fichiers restent dans l'application desktop. Avec WeChat, le téléphone devient lui aussi un point d'entrée pour envoyer des tâches et récupérer des fichiers.

## Tour d'horizon desktop

### Connexion

<img src="assets/screenshots/desktop-login.jpg" alt="MyCodex login" width="900">

- Connexion par numéro de téléphone et code de vérification.
- Acceptation des conditions générales et de la politique de confidentialité.
- Reprise de session automatique.
- Nouvelle tentative automatique en cas d'échec de connexion.

### Première configuration du modèle

<img src="assets/screenshots/desktop-model-setup.jpg" alt="MyCodex first model setup" width="900">

- Configuration recommandée via un compte d'abonnement.
- Configuration possible via clé API.
- Accès aux paramètres avancés si besoin.

### Conversation

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex conversation home" width="900">

- Décrire son objectif.
- Choisir un modèle et un projet.
- Joindre des images ou des fichiers.
- Démarrer depuis des scénarios préconçus.
- Interrompre une tâche en cours.

Les scénarios intégrés couvrent notamment la collecte de sujets tendance, la recherche de prospects, le rapport d'activité et la veille concurrentielle.

### Projets et historique

<img src="assets/screenshots/desktop-project-history.jpg" alt="MyCodex projects and history" width="900">

Projets, conversations et dossiers de résultats restent liés entre eux. Il est possible de créer, renommer, ouvrir un dossier, définir un projet par défaut et revenir à une conversation passée.

### Tâche en cours

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex running task" width="900">

L'interface affiche ce que fait l'Agent en temps réel. L'état et les événements peuvent être restaurés après un rechargement ou une réouverture de l'application.

### Résultats et fichiers

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex result" width="900">

MyCodex regroupe dans la même conversation le Markdown, les tableaux, les liens, les pièces jointes et les fichiers générés. Les questions suivantes s'appuient sur le contexte existant.

### Détail d'exécution

<img src="assets/screenshots/desktop-execution-process.jpg" alt="MyCodex execution process" width="900">

Lecture, recherche, synthèse, écriture de fichiers et chemins parcourus peuvent être inspectés à tout moment.

### Aperçu des fichiers

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex file preview" width="900">

Markdown, CSV, HTML, JSON, logs, XML, images et PDF peuvent être consultés directement dans le panneau latéral de l'application. Le téléchargement et l'ouverture avec l'application système sont pris en charge.

### Mobile / WeChat

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex WeChat mobile entry" width="900">

- Connecter un compte WeChat personnel.
- Générer un QR code.
- Envoyer des tâches depuis WeChat.
- Répondre `1/2/3` pour sélectionner une action du menu.
- Recevoir les fichiers générés directement dans WeChat.

### Paramètres

<img src="assets/screenshots/desktop-settings.jpg" alt="MyCodex settings" width="900">

Compte, modèles, test de connexion, activation, modèle par défaut, édition, suppression et état du runtime local sont tous regroupés dans les paramètres.

### Compte d'abonnement

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex subscription setup" width="900">

Les fournisseurs disponibles incluent Grok, Nous, ChatGPT / Codex, Gemini, MiniMax, Qwen, GitHub Copilot et Claude Max.

### Clé API

<img src="assets/screenshots/desktop-model-api-key.jpg" alt="MyCodex API Key setup" width="900">

Les utilisateurs disposant de leurs propres clés API peuvent choisir le fournisseur, le modèle, la clé API, le Base URL et le modèle par défaut.

## Téléchargement

Le code source n'est pas encore publié. Le dépôt met pour l'instant à disposition des installateurs packagés.

- macOS Apple Silicon : `MyCodex-0.6.1-mac-arm64.dmg` ou `MyCodex-0.6.1-mac-arm64.zip`
- macOS Intel : `MyCodex-0.6.1-mac-x64.dmg` ou `MyCodex-0.6.1-mac-x64.zip`
- Windows x64 : la version 0.6.1 intègre les améliorations de stabilité Windows, mais le zip Windows distribuable sera ajouté après le build cible du runtime Windows. En attendant, utilisez le paquet portable d'une ancienne version.

Téléchargement via [GitHub Releases](https://github.com/guo2001china/mycodex/releases).

## Communauté

Rejoignez la communauté pour contribuer à rendre MyCodex accessible au plus grand nombre.

Lors de l'ajout, indiquez `MyCodex` en note.

<img src="assets/mycodex-community-wechat.jpg" alt="Rejoindre la communauté MyCodex via QR code" width="260">

## État du projet

MyCodex est encore en accès anticipé. Il est conseillé de l'essayer d'abord dans un dossier de test ou sur un workflow non critique, puis de l'intégrer progressivement à des tâches plus importantes.