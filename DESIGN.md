# DESIGN.md — 席替えアプリ

> AI-DLC Inception フェーズ成果物。

---

## カラーパレット

| 用途 | クラス / 値 |
|------|------------|
| 背景 | `bg-gray-50` |
| カード | `bg-white` + `shadow-sm` + `rounded-xl` |
| アクセント | `blue-600` |
| 男子席 | `bg-sky-50` / ボーダー `border-sky-200` |
| 女子席 | `bg-rose-50` / ボーダー `border-rose-200` |
| 不明席 | `bg-gray-50` / ボーダー `border-gray-200` |
| 利用不可席 | `bg-gray-200` / テキスト `text-gray-400` |
| 固定席バッジ | `bg-amber-100 text-amber-700` |

## タイポグラフィ

- フォント: システムフォント（sans-serif）
- タイトル: `text-xl font-bold text-gray-800`
- セクション見出し: `text-sm font-semibold text-gray-600 uppercase tracking-wide`
- 本文: `text-sm text-gray-700`

## コンポーネント設計

### タブナビゲーション
- 3タブ: `生徒管理` / `座席設定` / `生成・履歴`
- アクティブ: `border-b-2 border-blue-600 text-blue-600`

### 座席カード
- サイズ: `min-w-[52px] min-h-[52px]`
- 丸角: `rounded-lg`
- ボーダー: `border`
- ホバー: `hover:ring-2 hover:ring-blue-300`

### ピル（タグ）
- 視力配慮: `bg-orange-100 text-orange-700 text-[10px] px-1 rounded`
- 固定: `bg-amber-100 text-amber-700 text-[10px] px-1 rounded`
- 前回同じ: `bg-red-100 text-red-600 text-[10px] px-1 rounded`

## スマホ対応

- レイアウト: `max-w-5xl mx-auto` で中央寄せ
- 座席グリッド: `overflow-x-auto` + `fitToScreen` (transform: scale)
- スピナー: `-` / 数値入力 / `+` のセット、`flex items-center gap-1`
