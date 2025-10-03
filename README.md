## 🔹 Routing

### Pages

pages/ ディレクトリから自動生成されるルーティングの仕組みを学ぶ。

### Dynamic Routes

[id].vue のような動的ルーティングの実装方法。

### Nested Routes

子ルート・レイアウトを活用してページ構成を整理する。

### Middleware

ページ遷移前に処理（認証チェック、ログなど）を挟む方法を学習。

## 🔹 Rendering

### SSR (Server-Side Rendering)

サーバーで HTML を生成して返す仕組みとメリット（SEO、初期表示速度）。

### CSR (Client-Side Rendering)

クライアントのみで動作するシングルページアプリの構成。

### SSG (Static Site Generation)

nuxt generate で静的サイトを生成する方法。ブログ・LP 向き。

### ISR (Incremental Static Regeneration)

一部ページをキャッシュしつつ、期限切れ後に再生成するハイブリッド戦略。

## 🔹 Data

### useFetch()

サーバー・クライアント両方から API を呼び出せるデータ取得フック。

### useAsyncData()

SSR 向けの非同期データ取得。キャッシュ戦略を理解する。

### Server API Routes

server/api/ ディレクトリで API エンドポイントを定義する方法。

### State (useState)

ページ間で共有できるグローバルステートを管理する仕組み。

### 🔹 UI & Composables

### useHead()

ページタイトルや meta タグを動的に設定。

### useSeoMeta()

SEO 最適化用の meta タグ設定。

### Teleport

DOM を別の場所に描画するテクニック（モーダルなどで活躍）。

### Suspense

非同期コンポーネントの読み込みを待機しつつ表示を制御。

## 🔹 Security

### Runtime Config

サーバーとクライアントで使える環境変数の管理。

### Server Middleware

リクエストに対するサーバー処理を挟む（ログ、CORS、認証）。

### Auth

認証フローの基本（Cookie、JWT、OAuth など）。

## 🔹 Modules

### Nuxt UI

UI コンポーネントライブラリ。ダッシュボードやフォームを素早く構築。

### Nuxt Image

画像最適化（レスポンシブ画像、WebP、自動変換）。

### Nuxt Content

Markdown ベースのコンテンツ管理。ドキュメントサイトやブログに最適。

### Third Party Modules

公式/非公式モジュールを導入して開発効率を上げる。

## ✅ 学習の進め方

### Routing → ページの基礎を理解

### Rendering → SSR/CSR/SSG の違いを把握

### Data → API やステート管理を実装

### UI & Composables → ページをリッチにする

### Security → 実用的なアプリに必要なセキュリティを追加

### Modules → Nuxt を拡張して本番レベルへ
