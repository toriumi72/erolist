# app/ README

このディレクトリは **Next.js App Router のルーティングと画面**の中心です。

## ここに置くもの

- `page.tsx` / `layout.tsx` / `loading.tsx` / `error.tsx` / `not-found.tsx`
- ルート（URL）単位の UI（基本は Server Components）
- **機能固有（専用）コンポーネント**: その機能の `page.tsx` と同階層に置く
- Server Actions（推奨: `app/_actions/` や各ルート配下に `actions.ts` などで配置）

## ここに置かないもの

- 再利用前提の汎用 UI（→ `components/`）
- 外部 API ラッパー・ビジネスロジック（→ `services/`）
- 初期化/クライアント生成などライブラリ固有コード（→ `lib/`）

## 典型例

- `app/(marketing)/page.tsx`
- `app/sites/page.tsx`（一覧）
- `app/sites/[id]/page.tsx`（詳細）
- `app/_actions/site-actions.ts`（Server Actions）


