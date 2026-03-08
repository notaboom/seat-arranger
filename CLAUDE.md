# CLAUDE.md — seat-arranger

> このファイルは `seat-arranger/` ディレクトリで作業する際のエージェント定義です。
> **ルートの `../CLAUDE.md` に定義されたグローバルルールをすべて継承・遵守します。**

---

## プロジェクト概要

- **アプリ名**: 席替えアプリ
- **形態**: 単一 `index.html`（React + Tailwind CDN / Babel）
- **公開先**: GitHub Pages
- **ターゲット**: スマホ（iPhone Safari）/ タブレット / PC

## 技術スタック

| 要素 | 内容 |
|------|------|
| フレームワーク | React 18 (CDN) |
| スタイル | Tailwind CSS v3 (CDN Play) |
| トランスパイル | Babel Standalone |
| データ保存 | localStorage |
| 外部通信 | なし |

## ファイル構成

```
seat-arranger/
├── index.html      # メインアプリ（単一ファイル、全コード含む）
├── SPEC.md         # 機能仕様書
├── DESIGN.md       # デザイン規約
├── README.md       # ユーザー向けガイド
├── CHANGELOG.md    # 変更履歴
└── CLAUDE.md       # 本ファイル
```

## 開発ルール

- `index.html` のみ編集すれば動作する構成を維持する
- CDN URL は変更しない（バージョン固定）
- localStorage キー: `seatArranger_v1`
