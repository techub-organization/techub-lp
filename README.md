# Tech Hub 開発部 LP

Tech Hub 開発部のランディングページです。  
`main` ブランチへの push をトリガーに GitHub Pages で自動公開されます。

公開URL:  
`https://techub-organization.github.io/techub-lp/`

## Overview

26卒の新卒が発起人となり立ち上がった「開発部」の紹介LP。  
Slackを拠点に、初心者から個人開発者、ビジネス職までが集うコミュニティの考え方・プロダクト・歩みを伝えます。

- 静的 HTML / CSS のみで構成（ビルド不要）
- GitHub Pages でそのままホスティング可能
- レスポンシブ対応（モバイル〜デスクトップ）

## Screenshot

![Tech Hub 開発部 LP トップビュー](assets/screenshots/home.png)

## Page Structure

| # | セクション | 内容 |
|---|---|---|
| 01 | Concept | 技術の深さより一歩目を歓迎する考え方。初心者・ビジネス職・個人開発者のすべてを対象にした姿勢とMotivationを紹介 |
| 02 | Values | Integrity / Grit / Challenge / Logic / AI-Standard / Well-being の6基準と、部活のPurposeを掲載 |
| 03 | Products | ReachTrail（フィーチャード）をはじめ、部員が開発・公開したプロダクトをカード形式で紹介 |
| 04 | Community | 26名参加・エンジニア職とビジネス職混在のコミュニティ構成を説明 |
| 05 | Progress | Slackチャンネル開設からGitHub Organization設立、LP制作開始までの軌跡を時系列で掲載 |
| — | Join Us | アイディア・技術・好奇心、それぞれの「欠片」を持ち寄る実験場としての呼びかけ |

## Products

現在掲載しているプロダクト:

- **ReachTrail** — Flutter MVP / Web・macOS 公開済み
- **Wording Stock** — SNS / Web 公開済み（PWA・Expo Go は今後対応予定）
- **Toriforium Portfolio** — Astro SSG + microCMS ポートフォリオ
- **LLM Google Calendar Extension** — Chrome/Edge 拡張（社内限定配布）
- **Dockerクイズページ** — React + Vite の学習サイト
- **Slackチャンネル分析bot** — 日報対応 Slack bot
- **AI仕様設計の検証** — AI による仕様書・提案書設計の検証
- **ccusage Discord bot** — AI使用率・リセット時間リマインドボット
- **Fudagit** — SolidJS 製 Git コマンド学習カルタゲーム
- **Portion-Flow** — 加重配分 Web ユーティリティ（ジニドル専用カスタマイズ）
- **cmdock** — Linux / Docker 学習用モック CLI ゲーム

## Files

```
techub-lp/
├── index.html                        # LP 本体
├── styles.css                        # デザイン・レイアウト・レスポンシブ定義
├── assets/
│   ├── favicons/                     # ファビコン（apple-touch-icon 等）
│   ├── icons/                        # ブランドアイコン（SVG / PNG）
│   └── screenshots/home.png         # README 用スクリーンショット
└── .github/workflows/deploy-pages.yml  # GitHub Pages デプロイ設定
```

## GitHub Pages

`main` への push でデプロイが自動実行されます。

初回のみ以下の設定が必要:

1. リポジトリの `Settings > Pages` を開く
2. `Build and deployment > Source` を `GitHub Actions` に設定する

## Local Preview

```bash
python3 -m http.server 8000
# → http://localhost:8000 で確認
```
