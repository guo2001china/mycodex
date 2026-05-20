# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

Codex + Hermes pour tout le monde : moins de friction autour des tokens, moins de configuration fragile, un workflow de bureau plus stable.

MyCodex transforme Codex + Hermes en espace de travail desktop. Vous ouvrez l'application, décrivez le résultat attendu, puis l'Agent exécute la tâche, affiche le déroulé et conserve les fichiers produits. Avec WeChat connecté, vous pouvez aussi envoyer des tâches et recevoir des fichiers depuis le téléphone.

## v0.7.0

- Private Browser Control est ajouté : l'Agent peut ouvrir et piloter une session navigateur isolée pour les tâches web, sans mélanger l'état du navigateur quotidien de l'utilisateur.
- Les tâches avec navigateur conservent un déroulé plus clair, avec navigation, lecture de pages et interactions visibles dans la conversation.
- Les améliorations de stabilité de 0.6.1 restent actives : timeouts cloud auth, relances sûres et adresse MyCodex de production dans les packages.
- Les packages macOS Apple Silicon et Intel sont reconstruits en 0.7.0.
- WeChat et Hermes restent le workflow principal : envoyer des tâches, continuer une conversation, recevoir les fichiers de résultat.
- Les résultats ne sont pas seulement une réponse : déroulé, conclusion, tableaux, fichiers et prochaines actions restent dans la même conversation.

## Le problème

Beaucoup de personnes veulent utiliser Codex + Hermes, mais s'arrêtent avant la première tâche utile à cause des tokens, du terminal, du routage de modèles et des variables d'environnement.

MyCodex réduit l'entrée à trois étapes : télécharger, se connecter, décrire la tâche. Les résultats, le processus et les fichiers restent dans l'application desktop. Avec WeChat, le téléphone peut aussi envoyer des tâches et recevoir des fichiers.

## Tour desktop

### Connexion

<img src="assets/screenshots/desktop-login.jpg" alt="MyCodex login" width="900">

- Connexion par téléphone et code de vérification.
- Acceptation des conditions et de la politique de confidentialité.
- Restauration de session.
- État de nouvelle tentative en cas d'erreur de connexion.

### Première configuration de modèle

<img src="assets/screenshots/desktop-model-setup.jpg" alt="MyCodex first model setup" width="900">

- Configuration par compte d'abonnement recommandée.
- Configuration par API Key disponible.
- Accès aux paramètres complets si nécessaire.

### Conversation

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex conversation home" width="900">

- Décrire l'objectif.
- Choisir un modèle et un projet.
- Ajouter des images ou fichiers.
- Démarrer depuis des scénarios courants.
- Arrêter une tâche en cours.

Les scénarios intégrés incluent la collecte de sujets tendance, la recherche de leads, le rapport d'opérations et la surveillance de concurrents.

### Projets et historique

<img src="assets/screenshots/desktop-project-history.jpg" alt="MyCodex projects and history" width="900">

Les projets, conversations et dossiers de résultats restent liés. On peut créer, renommer, ouvrir un dossier, définir un projet par défaut et revenir à une conversation passée.

### Tâche en cours

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex running task" width="900">

La page montre ce que fait l'Agent. L'état et les événements peuvent être restaurés après un rafraîchissement ou une réouverture.

### Résultats et fichiers

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex result" width="900">

MyCodex garde Markdown, tableaux, liens, pièces jointes et fichiers générés dans la même conversation. Les questions suivantes gardent le contexte.

### Détail d'exécution

<img src="assets/screenshots/desktop-execution-process.jpg" alt="MyCodex execution process" width="900">

Lecture, recherche, synthèse, écriture de fichiers et chemins touchés peuvent être inspectés.

### Private Browser Control

Quand une tâche a besoin du web, l'Agent peut piloter une session navigateur privée et séparée. Les ouvertures de pages, lectures, clics et autres interactions restent visibles dans le déroulé, tandis que les réponses et fichiers produits restent liés à la même conversation. La session peut être fermée à la fin de la tâche pour limiter le chevauchement avec le navigateur habituel.

### Aperçu de fichiers

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex file preview" width="900">

Markdown, CSV, HTML, JSON, logs, XML, images et PDF peuvent être consultés à droite dans l'application. Le téléchargement et l'ouverture avec l'application système sont pris en charge.

### Mobile / WeChat

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex WeChat mobile entry" width="900">

- Connecter un WeChat personnel.
- Générer un QR code.
- Envoyer des tâches depuis WeChat.
- Répondre `1/2/3` pour choisir une action de menu.
- Recevoir les fichiers générés dans WeChat.

### Paramètres

<img src="assets/screenshots/desktop-settings.jpg" alt="MyCodex settings" width="900">

Compte, modèles, test de connexion, activation, modèle par défaut, édition, suppression et état du runtime local sont regroupés dans les paramètres.

### Compte d'abonnement

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex subscription setup" width="900">

Les premières entrées incluent Grok, Nous, ChatGPT / Codex, Gemini, MiniMax, Qwen, GitHub Copilot et Claude Max.

### API Key

<img src="assets/screenshots/desktop-model-api-key.jpg" alt="MyCodex API Key setup" width="900">

Les utilisateurs avec leurs propres API Keys peuvent choisir le fournisseur, le modèle, l'API Key, le Base URL et le modèle par défaut.

## Télécharger

Le code source n'est pas encore publié. Le dépôt fournit d'abord des installateurs packagés.

- macOS Apple Silicon : `MyCodex-0.7.0-mac-arm64.dmg` ou `MyCodex-0.7.0-mac-arm64.zip`
- macOS Intel : `MyCodex-0.7.0-mac-x64.dmg` ou `MyCodex-0.7.0-mac-x64.zip`
- Windows x64 : l'asset Windows 0.7.0 sera ajouté après le build cible du runtime Windows. Pour l'instant, utilisez le package portable d'un ancien Release.

Téléchargement via [GitHub Releases](https://github.com/guo2001china/mycodex/releases).

## Communauté

Rejoignez la communauté pour rendre MyCodex plus accessible.

Lors de l'ajout, indiquez `MyCodex` en note.

<img src="assets/mycodex-community-wechat.jpg" alt="Join the MyCodex community QR code" width="260">

## Statut

MyCodex est encore en early preview. Essayez-le d'abord dans un dossier de test ou un workflow non critique, puis intégrez-le progressivement aux tâches importantes.
