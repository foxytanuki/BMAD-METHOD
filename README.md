# BMAD-METHOD™: 汎用AIエージェントフレームワーク

[![Version](https://img.shields.io/npm/v/bmad-method?color=blue&label=version)](https://www.npmjs.com/package/bmad-method)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Node.js Version](https://img.shields.io/badge/node-%3E%3D20.0.0-brightgreen)](https://nodejs.org)
[![Discord](https://img.shields.io/badge/Discord-Join%20Community-7289da?logo=discord&logoColor=white)](https://discord.gg/gk8jAdXWmj)

エージェンティック・アジャイル・ドリブン・デベロップメントの基盤、すなわちBreakthrough Method of Agile AI-Driven Development（画期的なアジャイルAI駆動開発手法）として知られていますが、それ以上の価値を提供します。特化したAIエクスパティーズによって、ソフトウェア開発、エンターテイメント、クリエイティブライティング、ビジネス戦略から個人のウェルネスまで、あらゆる領域を変革します。

**[BMadCodeのYouTubeチャンネルを登録](https://www.youtube.com/@BMadCode?sub_confirmation=1)**

**[Discordコミュニティに参加](https://discord.gg/gk8jAdXWmj)** - AIエンスージアスト向けの成長中のコミュニティです！困ったときのヘルプ、アイデアの共有、AIエージェントやフレームワークの探求、技術プロジェクトでのコラボレーション、趣味の共有、そして互いの成功のサポートを行っています。BModで困ったとき、独自のエージェントを構築したいとき、単にAIの最新動向について話したいとき - 私たちがサポートします！ **一部のモバイルやVPNではDiscordへの参加に問題が生じる場合があります。これはDiscordの問題です。招待リンクが機能しない場合は、自宅のネットワークや他のネットワーク、非VPN環境から試してください。**

⭐ **このプロジェクトが役立つ、または有用だと感じた場合は、右上の角にある星を付けてください！** これにより他の人がBMAD-METHOD™を発見しやすくなり、更新情報も受け取れるようになります！

## 概要

**BMAD-METHOD™の2つの主要なイノベーション：**

**1. エージェンティック・プランニング：** 専任のエージェント（アナリスト、PM、アーキテクト）があなたと協力して、詳細で一貫性のあるPRD（Product Requirements Document）とアーキテクチャ文書を作成します。高度なプロンプトエンジニアリングと人間参加型の改善プロセスを通じて、これらの計画エージェントは汎用的なAIタスク生成をはるかに超える包括的な仕様書を作成します。

**2. コンテキスト・エンジニアード・デベロップメント：** スクラムマスターエージェントが、これらの詳細な計画を、開発エージェントが必要とするすべてを含む超詳細な開発ストーリーに変換します - 完全なコンテキスト、実装の詳細、そしてアーキテクチャ・ガイダンスがストーリーファイルに直接埋め込まれます。

この2段階アプローチにより、AI支援開発における最大の問題である**計画の不整合**と**コンテキストの損失**の両方が解消されます。開発エージェントはストーリーファイルを開くと、何を構築し、どのように構築し、なぜ構築するのかを完全に理解できます。

**📖 [ユーザーガイドで完全なワークフローを確認](docs/user-guide.md)** - 計画フェーズ、開発サイクル、およびすべてのエージェントの役割

## クイックナビゲーション

### BMadワークフローの理解

**BMadの動作原理を説明するこれらの重要なワークフロー図を最初に確認してください：**

1. **[計画ワークフロー (Web UI)](docs/user-guide.md#the-planning-workflow-web-ui)** - PRDとアーキテクチャ文書の作成方法
2. **[コア開発サイクル (IDE)](docs/user-guide.md#the-core-development-cycle-ide)** - SM、Dev、QAエージェントがストーリーファイルを通じて協力する方法

> ⚠️ **これらの図は、BMad Methodのエージェンティックアジャイルフローの混乱の90%を説明しています** - PRD+アーキテクチャ作成とSM/Dev/QAワークフロー、そしてエージェントがストーリーファイルを通じてノートを渡す方法を理解することが不可欠であり、これがタスクマスターや単純なタスクランナーではないことも説明しています！

### 何をしたいですか？

- **[フルスタックアジャイルAIチームでソフトウェアをインストール・構築](#quick-start)** → クイックスタート手順
- **[BMadの使い方を学ぶ](docs/user-guide.md)** → 完全なユーザーガイドとウォークスルー
- **[利用可能なAIエージェントを見る](/bmad-core/agents)** → チームのための専門的な役割
- **[非技術的な用途を探る](#-beyond-software-development---expansion-packs)** → クリエイティブライティング、ビジネス、ウェルネス、教育
- **[独自のAIエージェントを作成](docs/expansion-packs.md)** → あなたの領域のためのエージェントを構築
- **[既製のエクスパンションパックを閲覧](expansion-packs/)** → ゲーム開発、DevOps、インフラストラクチャ、そしてアイデアと例からインスピレーションを得る
- **[アーキテクチャを理解](docs/core-architecture.md)** → 技術的な深掘り
- **[コミュニティに参加](https://discord.gg/gk8jAdXWmj)** → ヘルプを得てアイデアを共有

## 重要：BMadインストールを最新に保つ

**簡単に最新状態を保ちましょう！** プロジェクトにBMAD-METHOD™が既にインストールされている場合は、単純に以下を実行してください：

```bash
npx bmad-method install
# または
git pull
npm run install:bmad
```

これにより以下が行われます：

- ✅ 既存のv4インストールを自動検出
- ✅ 変更されたファイルのみを更新し、新しいファイルを追加
- ✅ カスタム変更に対して`.bak`バックアップファイルを作成
- ✅ プロジェクト固有の設定を保持

これにより、カスタマイズを失うことなく、最新の改善、バグ修正、新しいエージェントの恩恵を簡単に受けることができます！

## クイックスタート

### すべてを一つのコマンドで（IDE インストール）

**以下のコマンドのいずれかを実行するだけです：**

```bash
npx bmad-method install
# または明示的にstableタグを使用:
npx bmad-method@stable install
# またはBMadが既にインストールされている場合:
git pull
npm run install:bmad
```

この単一のコマンドで以下が処理されます：

- **新規インストール** - プロジェクトにBMadをセットアップ
- **アップグレード** - 既存のインストールを自動更新
- **エクスパンションパック** - package.jsonに追加したエクスパンションパックをインストール

> **それだけです！** 初回インストール、アップグレード、エクスパンションパックの追加のいずれの場合でも、これらのコマンドがすべてを行います。

**前提条件**: [Node.js](https://nodejs.org) v20+が必要です

### 最速スタート：Web UIフルスタックチームがあなたのものに（2分）

1. **バンドルを取得**: [フルスタックチームファイル](dist/teams/team-fullstack.txt)を保存またはクローンするか、他のチームを選択
2. **AIエージェントを作成**: 新しいGemini GemまたはCustomGPTを作成
3. **アップロードと設定**: ファイルをアップロードし、指示を設定：「重要な操作指示が添付されています。指示に従ってキャラクターを破らないでください」
4. **アイデア出しと計画を開始**: チャットを開始！ `*help`と入力して利用可能なコマンドを確認するか、`*analyst`のようなエージェントを選んでブリーフの作成を開始
5. **重要**: いつでもWeb上のBMad Orchestrator（#bmad-orchestratorコマンド）と話し、これがどのように機能するかについて質問してください！
6. **IDEに移行するタイミング**: PRD、アーキテクチャ、オプションのUXとブリーフができたら、IDEに切り替えて文書をシャード化し、実際のコードの実装を開始します！詳細は[ユーザーガイド](docs/user-guide.md)をご覧ください

### 代替案：クローンとビルド

```bash
git clone https://github.com/bmadcode/bmad-method.git
npm run install:bmad # すべてを宛先フォルダにビルドしてインストール
```

## 🌟 ソフトウェア開発を超えて - エクスパンションパック

BMAD™の自然言語フレームワークはあらゆる領域で動作します。エクスパンションパックは、クリエイティブライティング、ビジネス戦略、健康とウェルネス、教育などの専門的なAIエージェントを提供します。また、エクスパンションパックは、すべてのケースに汎用的ではない特定の機能でコアBMAD-METHOD™を拡張することができます。[エクスパンションパックガイド](docs/expansion-packs.md)をご覧いただき、独自のものを作成する方法を学んでください！

## コードベースフラットナーツール

BMAD-METHOD™には、プロジェクトファイルをAIモデルが消費できるように準備する強力なコードベースフラットナーツールが含まれています。このツールは、コードベース全体を単一のXMLファイルに集約し、分析、デバッグ、開発支援のためにプロジェクトのコンテキストをAIアシスタントと簡単に共有できるようにします。

### 機能

- **AI最適化出力**: AIモデルの消費に特化して設計されたクリーンなXML形式を生成
- **スマートフィルタリング**: `.gitignore`パターンを自動的に尊重し、不要なファイルを除外
- **バイナリファイル検出**: バイナリファイルを智的に識別して除外し、ソースコードに焦点を当てる
- **進捗追跡**: リアルタイム進捗インジケータと包括的な完了統計
- **柔軟な出力**: カスタマイズ可能な出力ファイルの場所と命名

### 使用方法

```bash
# 基本的な使用法 - 現在のディレクトリにflattened-codebase.xmlを作成
npx bmad-method flatten

# カスタム入力ディレクトリを指定
npx bmad-method flatten --input /path/to/source/directory
npx bmad-method flatten -i /path/to/source/directory

# カスタム出力ファイルを指定
npx bmad-method flatten --output my-project.xml
npx bmad-method flatten -o /path/to/output/codebase.xml

# 入力と出力オプションを組み合わせ
npx bmad-method flatten --input /path/to/source --output /path/to/output/codebase.xml
```

### 出力例

ツールは進捗を表示し、包括的な要約を提供します：

```text
📊 完了サマリー:
✅ 156個のファイルをflattened-codebase.xmlに正常に処理
📁 出力ファイル: /path/to/your/project/flattened-codebase.xml
📏 総ソースサイズ: 2.3 MB
📄 生成されたXMLサイズ: 2.1 MB
📝 総コード行数: 15,847
🔢 推定トークン数: 542,891
📊 ファイル内訳: テキスト142、バイナリ14、エラー0
```

生成されたXMLファイルには、AIモデルが簡単に解析して理解できる構造化された形式でプロジェクトのテキストベースのソースファイルが含まれており、コードレビュー、アーキテクチャ討議、またはBMAD-METHOD™プロジェクトでのAIアシスタンスの取得に最適です。

#### 高度な使用方法とオプション

- CLIオプション
  - `-i, --input <path>`: フラット化するディレクトリ。デフォルト：現在の作業ディレクトリまたはインタラクティブ実行時の自動検出されたプロジェクトルート。
  - `-o, --output <path>`: 出力ファイルパス。デフォルト：選択されたディレクトリの`flattened-codebase.xml`。
- インタラクティブモード
  - `--input`と`--output`を渡さず、ターミナルがインタラクティブ（TTY）の場合、ツールはプロジェクトルートの検出を試み（`.git`、`package.json`などのマーカーを探して）、パスの確認または上書きを促します。
  - 非インタラクティブなコンテキスト（例：CI）では、検出されたルートを静かに優先し、そうでなければ現在のディレクトリとデフォルトファイル名にフォールバックします。
- ファイル発見と無視
  - gitリポジトリ内では速度と正確性のために`git ls-files`を使用し、そうでなければglobベースのスキャンにフォールバックします。
  - `.gitignore`に加えて、厳選されたデフォルトの無視パターン（例：`node_modules`、ビルド出力、キャッシュ、ログ、IDEフォルダ、ロックファイル、大きなメディア/バイナリ、`.env*`、以前に生成されたXML出力）を適用します。
- バイナリ処理
  - バイナリファイルは検出され、XMLコンテンツから除外されます。最終サマリーでカウントされますが、出力に埋め込まれません。
- XML形式と安全性
  - ルート要素`<files>`を持つUTF-8エンコードファイル。
  - 各テキストファイルは、`<![CDATA[ ... ]]>`でラップされたコンテンツを持つ`<file path="relative/path">`要素として出力されます。
  - ツールは、CDATAを分割することでコンテンツ内の`]]>`の出現を安全に処理し、正確性を保持します。
  - ファイルの内容はそのまま保持され、XML内で読みやすさのためにインデントされます。
- パフォーマンス
  - 同時実行数は、CPUとワークロードサイズに基づいて自動的に選択されます。設定は不要です。
  - gitリポジトリ内での実行により、発見パフォーマンスが向上します。

#### 最小限のXML例

```xml
<?xml version="1.0" encoding="UTF-8"?>
<files>
  <file path="src/index.js"><![CDATA[
    // あなたのソースコンテンツ
  ]]></file>
</files>
```

## ドキュメントとリソース

### 必須ガイド

- 📖 **[ユーザーガイド](docs/user-guide.md)** - プロジェクトの開始から完了までの完全なウォークスルー
- 🏗️ **[コアアーキテクチャ](docs/core-architecture.md)** - 技術的な深掘りとシステム設計
- 🚀 **[エクスパンションパックガイド](docs/expansion-packs.md)** - ソフトウェア開発を超えたあらゆる領域にBMadを拡張

## サポート

- 💬 [Discordコミュニティ](https://discord.gg/gk8jAdXWmj)
- 🐛 [問題追跡](https://github.com/bmadcode/bmad-method/issues)
- 💬 [ディスカッション](https://github.com/bmadcode/bmad-method/discussions)

## 貢献

**貢献を歓迎し、あなたのアイデア、改善、エクスパンションパックを心から歓迎します！** 🎉

📋 **[CONTRIBUTING.mdをお読みください](CONTRIBUTING.md)** - ガイドライン、プロセス、要件を含む貢献の完全なガイド

### フォークでの作業

このリポジトリをフォークすると、リソースを節約するためにCI/CDワークフローは**デフォルトで無効**になります。これは意図的であり、フォークをクリーンに保つのに役立ちます。

#### フォークでCI/CDが必要ですか？

フォークでワークフローを有効にする方法については、[フォークCI/CDガイド](.github/FORK_GUIDE.md)をご覧ください。

#### 貢献ワークフロー

1. **リポジトリをフォーク** - GitHubのForkボタンをクリック
2. **フォークをクローン** - `git clone https://github.com/YOUR-USERNAME/BMAD-METHOD.git`
3. **機能ブランチを作成** - `git checkout -b feature/amazing-feature`
4. **変更を行う** - `npm test`でローカルテスト
5. **変更をコミット** - `git commit -m 'feat: add amazing feature'`
6. **フォークにプッシュ** - `git push origin feature/amazing-feature`
7. **プルリクエストを開く** - CI/CDがPR上で自動実行されます

PR提出時に貢献がテストされます - フォークでCIを有効にする必要はありません！

## ライセンス

MITライセンス - 詳細は[LICENSE](LICENSE)をご覧ください。

## 商標表示

BMAD™およびBMAD-METHOD™は、BMad Code, LLCの商標です。無断転載を禁じます。

[![Contributors](https://contrib.rocks/image?repo=bmadcode/bmad-method)](https://github.com/bmadcode/bmad-method/graphs/contributors)

<sub>AI支援開発コミュニティのために❤️で構築</sub>
