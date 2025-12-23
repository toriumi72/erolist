# hooks/ README

このディレクトリは **再利用可能なカスタム React Hooks** を置きます。

## ここに置くもの

- `useSWR` を使ったデータ取得 Hooks（ユーザー操作に依存するデータ向け）
- UI 状態の共通ロジック（ただし URL 状態は `nuqs` に寄せる）
- 複数画面で共有したい Hook

## ここに置かないもの

- DB 直アクセス（禁止。必ず Server Actions 経由）
- 特定ページ専用 Hook（→ そのページと同階層でも可）

## 典型例

- `hooks/use-sites.ts`（一覧取得 + mutate）
- `hooks/use-search-params.ts`（nuqs ラッパー）


