# components/ README

このディレクトリは **汎用 UI コンポーネント置き場**です（再利用可能・ロジック最小）。

## ここに置くもの

- shadcn/ui ベースの **再利用可能な UI**（ボタン、カード、テーブル等）
- **ドメインに依存しない** Presentational Components
- `cn()` 等の UI 付随ユーティリティ（ただし一般ユーティリティは `utils/`）

## ここに置かないもの

- サーバー処理 / Server Actions（→ `app/` 側）
- DB 接続や外部 API 呼び出し（→ `services/` / `lib/`）
- 特定ページ専用コンポーネント（→ 対応する `app/.../page.tsx` と同階層）

## 典型例

- `components/ui/button.tsx`
- `components/site-card.tsx`（汎用的に使える場合のみ）


