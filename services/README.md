# services/ README

このディレクトリは **ビジネスロジック** と **外部サービス連携（API ラッパー）** を置きます。

## ここに置くもの

- 例: サイト一覧取得、ランキング計算、検索条件の適用などのユースケース
- 外部 API の呼び出しラッパー
- Server Actions から呼ばれる「目的が明確な処理」

## 重要ルール

- DB 接続/クエリは **サーバー側のみ**。Client Components から直接呼ばない
- ただし、Server Actions にすべての実装をベタ書きせず、`services/` に寄せて見通しをよくする

## ここに置かないもの

- UI コンポーネント（→ `components/` / `app/`）
- 何でもできる汎用サービス（多目的なサーバー関数）は避ける

## 典型例

- `services/sites/get-sites.ts`
- `services/rankings/get-ranking.ts`


