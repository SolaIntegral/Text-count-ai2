---
project: Contäx
status: in-progress
created: 2026-04-07
---

# Contäx

## 概要
AIを活用したブロック型テキストエディタアプリ。
「AIへの思い込みを取り除く」をコンセプトに、ユーザーが感じる文章作成の心理的障壁を外す。

## コードの場所
リポジトリルート（`docx/` に技術ドキュメント、`docs/` にプロダクト・事業ドキュメント）

## 現在の技術スタック
- **フレームワーク**: Next.js 16（App Router）
- **スタイル**: Tailwind CSS v4（shadcn/ui なし → 再構築で追加）
- **状態管理**: Zustand
- **DB**: Drizzle ORM + LibSQL
- **認証**: better-auth
- **D&D**: dnd-kit

## 再構築方針（2026-04-07〜）

### デザインシステム適用
- shadcn/ui を導入（プロダクト部署標準に準拠）
- フォント: Noto Sans JP
- プライマリーカラー: ブルー（oklch(0.546 0.245 262)）

### ロジック方針
- 既存のDB・認証・Zustand storeはそのまま維持
- UIコンポーネントのみ再構築

### マネタイズ追加（Phase 2）
- 決済機能の追加
- フリーミアム / サブスクモデルの設計
- → 詳細は `marketing/monetization/contax.md` を参照

## レイアウト構成
```
┌─────────────────────────────┐
│ TargetInput（文字数目標）    │
├──────────────┬──────────────┤
│ HintsBlock   │  BlockList   │
│（AIヒント）  │（テキスト）  │
├──────────────┴──────────────┤
│ EditorFooter                │
└─────────────────────────────┘
```

## 関連
- PMチケット: `pm/tickets/2026-04-07-contax-rebuild.md`
- マネタイズ: `marketing/monetization/contax.md`
