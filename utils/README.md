# utils/ README

このディレクトリは **アプリ全体で使える純粋なユーティリティ関数**を置きます。

## ここに置くもの

- 日付/文字列/配列などの変換・整形
- フォーマッタ、バリデーション補助（Zod スキーマ自体は用途により `types/` or 機能配下）
- 依存が少なく副作用のない関数

## ここに置かないもの

- UI コンポーネント（→ `components/`）
- DB/外部 API 呼び出し（→ `services/` / `lib/`）
- React Hook（→ `hooks/`）

## 典型例

- `utils/format-score.ts`
- `utils/paginate.ts`


