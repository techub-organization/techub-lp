# Tech Hub 開発部 LP

Tech Hub 開発部のランディングページです。  
`main` ブランチに push された静的ファイルを GitHub Pages で公開する前提の構成です。

公開URL:
`https://techub-organization.github.io/techub-lp/`

## Overview

- Slackチャンネルを起点にした Tech Hub 開発部の紹介LP
- 初心者、個人開発者、ビジネス職まで混ざるコミュニティを伝える構成
- 静的HTML / CSSベースのシンプルな実装
- GitHub Pages でそのまま配信できる構成

## Screenshot

トップビューのスクリーンショット:

![Tech Hub 開発部 LP トップビュー](assets/screenshots/home.png)

## Page Structure

このLPは以下のセクションで構成しています。

1. Hero
   Slack起点の部活であること、参加対象、承認待ちのステータスを最初に提示します。
2. Concept
   初心者歓迎、ビジネス職歓迎、個人開発歓迎という考え方を整理しています。
3. Values
   Integrity / Grit / Challenge / Logic / AI-Standard / Well-being を掲載しています。
4. Products
   Reachtrail、Wordock、ポートフォリオサイト、Chrome拡張、Androidアプリなど、プロダクト単位で紹介しています。
5. Community
   部長と管轄人事を除いた25名参加、エンジニア職とビジネス職の混在を説明しています。
6. Progress
   チャンネル開設から公式化申請までの流れを時系列で掲載しています。

## Files

- `index.html`: LP本体
- `styles.css`: デザイン、レイアウト、レスポンシブ定義
- `Techub.png`: ヘッダーロゴ
- `assets/screenshots/home.png`: README用スクリーンショット
- `.github/workflows/deploy-pages.yml`: GitHub Pages デプロイ設定

## GitHub Pages

このリポジトリには、`main` への push をトリガーに GitHub Pages へデプロイする workflow を追加しています。

必要な初回設定:

1. GitHub リポジトリの `Settings` を開く
2. `Pages` を開く
3. `Build and deployment` の `Source` を `GitHub Actions` にする

設定後は、`main` に push されるたびに最新LPが公開されます。

## Local Preview

ローカル確認はシンプルに `index.html` をブラウザで開けば十分です。

必要に応じて簡易HTTPサーバーを使う場合:

```bash
python3 -m http.server 8000
```
