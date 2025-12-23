# types/ README

このディレクトリは **型定義（TypeScript）** を集約します。

## ここに置くもの

- ドメインモデル（例: Site / Review / Tag など）の型
- API/Server Actions の入出力型（共有したい場合）
- Zod スキーマ（プロジェクト方針として集約する場合）

## ここに置かないもの

- 実装（関数/クラス）主体のコード（→ `utils/` / `services/`）
- 画面専用のローカル型（→ その `page.tsx` 付近で定義でOK）

## 典型例

- `types/site.ts`
- `types/ranking.ts`


