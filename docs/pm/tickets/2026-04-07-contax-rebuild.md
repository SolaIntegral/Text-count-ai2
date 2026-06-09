---
status: in-progress
priority: high
created: 2026-04-07
project: contax
---

# Contäx 再構築チケット

## Phase 1: デザインシステム適用
- [x] shadcn/ui インストール・初期設定 | 完了: 2026-04-07
- [x] Noto Sans JP フォント設定 | 完了: 2026-04-07
- [x] プライマリーカラー（ブルー: oklch(0.546 0.245 262)）設定 | 完了: 2026-04-07
- [x] globals.css 更新（紫グラデ廃止）| 完了: 2026-04-07
- [x] サイドバー再構築（shadcn/ui Sheet・Button・Avatar・Separator・Tooltip）| 完了: 2026-04-07
- [x] エディターフッター再構築（Button コンポーネント統一）| 完了: 2026-04-07
- [x] ヒントブロック再構築（紫→ブルー統一）| 完了: 2026-04-07
- [x] ブロックカード・タイトルブロック 色統一 | 完了: 2026-04-07
- [ ] その他ページ（documents・templates・experiences）のUI確認・統一

## Phase 0: バグ修正（Phase 1より先にやる）
- [x] ヒントが別タブで消えるバグ修正（editor-store.tsのpartializeにhintsを追加）| 完了: 2026-04-07
- [x] 文字数オーバー時に結論が消えるバグ修正（prompts.ts + route.tsの改修）| 完了: 2026-04-07

## Phase 2: マネタイズ実装
- [ ] マネタイズ戦略確定（marketing/monetization/contax.md）
- [ ] Stripe 導入
- [ ] フリーミアムプランの制限ロジック実装
- [ ] 課金ページUI
