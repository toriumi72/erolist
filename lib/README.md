# lib/ README

このディレクトリは **ライブラリ固有の初期化・設定・クライアント生成**などを置きます。

## ここに置くもの

- Supabase / DB / 検索基盤などの **クライアント生成**（サーバー側）
- 外部 SDK の初期化、設定ラッパー
- ライブラリ依存の薄いユーティリティ（例: `lib/utils.ts` の `cn` など）

## 重要ルール

- **DB への接続は必ずサーバーサイド**で行う（Client Components から直接接続しない）

## ここに置かないもの

- 具体的なビジネスロジック（→ `services/`）
- ページ固有の UI（→ `app/`）

## 典型例

- `lib/supabase/server.ts`（サーバー用クライアント）
- `lib/supabase/middleware.ts`（必要なら）


