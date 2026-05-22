# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

Codex + Hermes für alle: weniger Token-Stress, weniger fragile Setups, ein stabilerer Desktop-Workflow.

MyCodex verpackt Codex + Hermes als Desktop-Arbeitsplatz. Du öffnest die App, beschreibst das gewünschte Ergebnis, und der Agent führt die Aufgabe aus, zeigt den Ablauf und speichert Ergebnisdateien. Über WeChat lassen sich Aufgaben auch vom Smartphone aus senden und Dateien zurückerhalten.

## v0.9.6

- Das Desktop-Hauptfenster wird stabiler verwaltet: Login-Callbacks, Update-Status und Fokusaktionen werden nicht mehr an bereits geschlossene Fenster gesendet.
- Externe Links, Login-Callbacks und ein zweiter App-Start stellen ein vorhandenes lebendes Fenster wieder her und fokussieren es.
- Minimierte Fenster werden vor dem Fokus wiederhergestellt, damit die App nicht unsichtbar weiterläuft.
- macOS Apple Silicon und macOS Intel wurden als 0.9.6 neu gebaut.
- Windows x64 bleibt bis zum nächsten Windows-Runtime-Build als 0.9.0-Archivpaket verfügbar.
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

### Real Browser Control

MyCodex kann den Agent über eine von der Desktop-App verwaltete Browsererweiterung mit einer echten Browsersitzung verbinden. Verbindungsstatus, aktive Sitzung, Erweiterungsversion und letzte Aktionen sind sichtbar, und Aufgaben mit Browser-Tool lassen sich direkt aus dem Composer starten.

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

- macOS Apple Silicon: `MyCodex-0.9.6-mac-arm64.dmg` oder `MyCodex-0.9.6-mac-arm64.zip`
- macOS Intel: `MyCodex-0.9.6-mac-x64.dmg` oder `MyCodex-0.9.6-mac-x64.zip`
- Windows x64: `MyCodex-0.9.0-win-x64.zip` bleibt im v0.9.0-Archiv verfügbar

Download über [GitHub Releases](https://github.com/guo2001china/mycodex/releases).

## Community

Hilf mit, MyCodex zugänglicher zu machen.

Bitte beim Hinzufügen als Notiz `MyCodex` angeben.

<img src="assets/mycodex-community-wechat.jpg" alt="Join the MyCodex community QR code" width="260">

## Status

MyCodex ist noch eine frühe Preview. Erst in einem Testordner oder einem unkritischen Workflow ausprobieren, danach schrittweise in wichtige Abläufe übernehmen.
