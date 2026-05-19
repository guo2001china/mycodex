# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

誰でも無料で使える Codex + Hermes。Token や複雑な環境設定に悩まされず、安定したワークフローを作るためのデスクトップ版です。

MyCodex は Codex + Hermes を、普通のユーザーがそのまま使える作業台としてまとめたものです。アプリを開き、やりたいことを伝えると、Agent が処理を進め、途中経過を見せ、結果ファイルを残します。WeChat を接続すれば、PC の前にいない時でもタスクを投げたり、結果ファイルを受け取ったりできます。

## v0.6.1 のポイント

- cloud auth 接続にタイムアウトと安全な再試行を追加し、短いネットワーク不調に強くしました。
- 配布用デスクトップパッケージに本番 MyCodex 接続設定を入れ、初回起動時の接続失敗を減らしました。
- Windows の安定運用に向け、完全な zip 構成、runtime 配置、パッケージ設定を検査する流れを追加しました。
- macOS Apple Silicon と Intel の 0.6.1 パッケージを更新しました。
- WeChat と Hermes のワークフローは引き続き中心です。タスク送信、会話継続、結果ファイル受信に使えます。
- 結果は単なる返答ではなく、過程、結論、表、ファイル、次のアクションまで同じ会話に残ります。

## 何を解決するか

Codex + Hermes を使いたい人は多いのに、Token、コマンドライン、モデル設定、環境変数で止まってしまうことがよくあります。

MyCodex は入口を「ダウンロード、ログイン、タスクを書く」の 3 ステップにします。結果、処理過程、生成ファイルはデスクトップに残ります。WeChat を接続すれば、スマホからもタスクを投げられます。

## 画面紹介

### ログイン

<img src="assets/screenshots/desktop-login.jpg" alt="MyCodex login" width="900">

- 携帯番号の認証コードでログイン。
- 利用規約とプライバシーポリシーの確認。
- ログイン状態の復元。
- 接続エラー時の再試行。

### 初回モデル接続

<img src="assets/screenshots/desktop-model-setup.jpg" alt="MyCodex model setup" width="900">

- サブスクリプションアカウント接続を推奨。
- API Key 接続も選択可能。
- 詳細設定ページにも移動できます。

### 会話ホーム

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex conversation home" width="900">

- タスクの目的を入力。
- モデルとプロジェクトを選択。
- 画像やファイルを添付。
- よく使う業務シナリオから開始。
- 実行中のタスクを停止可能。

組み込みシナリオには、人気トピック整理、営業リード収集、運用レポート生成、競合変化の監視があります。

### プロジェクトと履歴

<img src="assets/screenshots/desktop-project-history.jpg" alt="MyCodex projects and history" width="900">

- プロジェクト作成、名前変更、フォルダを開く、既定プロジェクト設定。
- 過去の会話を開く、削除する。
- 実行中の会話は状態が表示されます。

### 実行中

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex running task" width="900">

Agent が何をしているかを画面上で確認できます。ページを更新した後でも、進行状態とイベントを復元できます。

### 結果と生成ファイル

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex result" width="900">

- 最終結果を表示。
- Markdown、表、リンクに対応。
- 添付ファイルと生成ファイルを同じ会話で管理。
- 文脈を保ったまま追加質問できます。

### 実行過程

<img src="assets/screenshots/desktop-execution-process.jpg" alt="MyCodex execution process" width="900">

読み取り、検索、要約、ファイル作成など、Agent が実行した操作を確認できます。

### ファイルプレビュー

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex file preview" width="900">

Markdown、CSV、HTML、JSON、ログ、XML、画像、PDF などを右側で確認できます。ダウンロードやシステムアプリで開く操作にも対応しています。

### モバイル / WeChat

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex WeChat mobile entry" width="900">

- 個人 WeChat の接続状態を確認。
- QR コードを生成。
- WeChat からタスク送信。
- `1/2/3` の返信でメニュー操作。
- 生成されたファイルを WeChat に返送。

### 設定

<img src="assets/screenshots/desktop-settings.jpg" alt="MyCodex settings" width="900">

- ログイン状態。
- モデル一覧、接続確認、有効化、既定設定、編集、削除。
- ローカル runtime の URL、バージョン、Agent 状態、データディレクトリ、結果ディレクトリ。

### サブスクリプションアカウント接続

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex subscription model setup" width="900">

Grok、Nous、ChatGPT / Codex、Gemini、MiniMax、Qwen、GitHub Copilot、Claude Max などの入口を用意しています。

### API Key 接続

<img src="assets/screenshots/desktop-model-api-key.jpg" alt="MyCodex API Key setup" width="900">

自分の API Key を使いたいユーザーは、提供元、モデル、API Key、Base URL、既定モデル設定を指定できます。

## ダウンロード

ソースコードはまだ公開していません。まずはパッケージ済みインストーラを配布しています。

- macOS Apple Silicon: `MyCodex-0.6.1-mac-arm64.dmg` または `MyCodex-0.6.1-mac-arm64.zip`
- macOS Intel: `MyCodex-0.6.1-mac-x64.dmg` または `MyCodex-0.6.1-mac-x64.zip`
- Windows x64: 0.6.1 には Windows 安定運用の改善が入っていますが、配布用 Windows zip は Windows runtime の target build 後に追加予定です。現時点では過去 Release の portable パッケージを使用してください。

[GitHub Releases](https://github.com/guo2001china/mycodex/releases) からダウンロードできます。

## コミュニティ

MyCodex をより多くの人が使えるものにするため、コミュニティに参加してください。

追加時の備考には `MyCodex` と書いてください。

<img src="assets/mycodex-community-wechat.jpg" alt="Join the MyCodex community QR code" width="260">

## 状態

MyCodex はまだ early preview です。まずはテスト用フォルダや重要度の低いワークフローで試してください。
