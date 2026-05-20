# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

Codex + Hermes für alle: weniger Token-Stress, weniger fragile Setups, ein stabilerer Desktop-Workflow.

MyCodex verpackt Codex + Hermes als Desktop-Arbeitsplatz. Du öffnest die App, beschreibst das gewünschte Ergebnis, und der Agent führt die Aufgabe aus, zeigt den Ablauf und speichert Ergebnisdateien. Über WeChat lassen sich Aufgaben auch vom Smartphone aus senden und Dateien zurückerhalten.

## v0.8.0

- Die Einstellungen enthalten jetzt Agent-Konfiguration: Standardrechte, Tool-Umfang, Netzwerkzugriff und maximale Laufzeit.
- Der Runtime-Bereich zeigt aktive Aufgaben, kann den Status aktualisieren und alle laufenden Aufgaben stoppen.
- Der Runtime-Status zeigt das Hermes-Datenverzeichnis, um lokale Agent-Authentifizierung und Laufzeitumgebung leichter zu prüfen.
- Die Gesprächsliste zeigt Statusmarker nur noch für laufende, wartende, fehlgeschlagene und gestoppte Gespräche.
- macOS Apple Silicon und Intel wurden als 0.8.0 neu gebaut.
- WeChat und Hermes bleiben der Kern-Workflow: Aufgaben senden, Gespräche fortsetzen, Ergebnisdateien empfangen.
- Ergebnisse bleiben als Arbeitsnachweis erhalten: Ablauf, Fazit, Tabellen, Dateien und nächste Schritte in derselben Unterhaltung.

## Warum

Viele Nutzer wollen Codex + Hermes nutzen, brechen aber bei Token, Kommandozeile, Modellrouting und Umgebungsvariablen ab.

MyCodex reduziert den Einstieg auf drei Schritte: herunterladen, einloggen, Aufgabe beschreiben. Ergebnisse, Prozess und Dateien bleiben in der Desktop-App. Mit WeChat lassen sich Aufgaben und Dateien auch mobil weiterführen.

## Desktop-Überblick

### Login

<img src="assets/screenshots/desktop-login.jpg" alt="MyCodex login" width="900">

- Login per Telefonnummer und Verifizierungscode.
- Zustimmung zu Nutzungsbedingungen und Datenschutz.
- Wiederherstellung bestehender Sessions.
- Retry-Zustand bei Verbindungsproblemen.

### Erstes Modell-Setup

<img src="assets/screenshots/desktop-model-setup.jpg" alt="MyCodex first model setup" width="900">

- Subscription-Account als empfohlener Weg.
- API-Key-Setup bleibt möglich.
- Direkter Einstieg in die vollständigen Einstellungen.

### Konversation

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex conversation home" width="900">

- Aufgabe eingeben.
- Modell und Projekt auswählen.
- Bilder oder Dateien anhängen.
- Mit typischen Szenarien starten.
- Laufende Aufgabe stoppen.

Typische Szenarien: Trendthemen sammeln, Sales-Leads recherchieren, Operations-Report erstellen, Wettbewerberänderungen beobachten.

### Projekte und Verlauf

<img src="assets/screenshots/desktop-project-history.jpg" alt="MyCodex projects and history" width="900">

Projekte, Gespräche und Ergebnisordner bleiben zusammen. Nutzer können Projekte anlegen, umbenennen, Ordner öffnen, Standardprojekte setzen und alte Gespräche wieder öffnen.

### Laufende Aufgaben

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex running task" width="900">

Der Agent zeigt, was gerade passiert. Laufende Zustände und Prozessereignisse können nach Refresh oder erneutem Öffnen wiederhergestellt werden.

### Ergebnisse und Dateien

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex result" width="900">

MyCodex zeigt Markdown, Tabellen, Links, Anhänge und generierte Dateien in derselben Unterhaltung. Anschlussfragen behalten den Kontext.

### Ablauf prüfen

<img src="assets/screenshots/desktop-execution-process.jpg" alt="MyCodex execution process" width="900">

Lesen, Suchen, Zusammenfassen, Schreiben von Dateien und berührte Pfade lassen sich einsehen.

### Agent-Einstellungen und Runtime-Kontrolle

MyCodex gibt Nutzern mehr Kontrolle darüber, wie der Agent läuft und welche Werkzeuge er verwenden darf. Standardrechte, Tool-Umfang, Netzwerkzugriff und maximale Laufzeit sind einstellbar. In den Einstellungen lassen sich aktive Runtime-Aufgaben aktualisieren oder stoppen, und das Hermes-Datenverzeichnis hilft bei lokaler Authentifizierung und Runtime-Diagnose.

### Dateivorschau

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex file preview" width="900">

Markdown, CSV, HTML, JSON, Logs, XML, Bilder und PDFs können direkt rechts in der App angesehen werden. Download und Öffnen mit System-Apps werden unterstützt.

### Mobile / WeChat

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex WeChat mobile entry" width="900">

- WeChat verbinden.
- QR-Code erzeugen.
- Aufgaben aus WeChat senden.
- Mit `1/2/3` Menüaktionen auswählen.
- Ergebnisdateien zurück in WeChat erhalten.

### Einstellungen

<img src="assets/screenshots/desktop-settings.jpg" alt="MyCodex settings" width="900">

Account, Modellliste, Modellprüfung, Aktivieren/Deaktivieren, Standardmodell, Bearbeiten, Löschen und lokaler Runtime-Status liegen in den Einstellungen.

### Subscription-Account

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex subscription setup" width="900">

Erste Einstiege umfassen Grok, Nous, ChatGPT / Codex, Gemini, MiniMax, Qwen, GitHub Copilot und Claude Max.

### API Key

<img src="assets/screenshots/desktop-model-api-key.jpg" alt="MyCodex API Key setup" width="900">

Wer eigene API Keys nutzt, kann Provider, Modell, API Key, Base URL und Standardmodell selbst festlegen.

## Download

Der Quellcode ist noch nicht veröffentlicht. Aktuell gibt es zuerst gepackte Installer.

- macOS Apple Silicon: `MyCodex-0.8.0-mac-arm64.dmg` oder `MyCodex-0.8.0-mac-arm64.zip`
- macOS Intel: `MyCodex-0.8.0-mac-x64.dmg` oder `MyCodex-0.8.0-mac-x64.zip`
- Windows x64: Das Windows-Asset für 0.8.0 folgt nach dem Target-Build der Windows-Runtime. Bis dahin das portable Paket aus einem früheren Release nutzen.

Download über [GitHub Releases](https://github.com/guo2001china/mycodex/releases).

## Community

Hilf mit, MyCodex zugänglicher zu machen.

Bitte beim Hinzufügen als Notiz `MyCodex` angeben.

<img src="assets/mycodex-community-wechat.jpg" alt="Join the MyCodex community QR code" width="260">

## Status

MyCodex ist noch eine frühe Preview. Erst in einem Testordner oder einem unkritischen Workflow ausprobieren, danach schrittweise in wichtige Abläufe übernehmen.
