# Favorite Recipes

お気に入りレシピを管理する静的Webサイト。
単一のHTMLファイル（HTML / CSS / JavaScript）で構成され、Vercel で公開しています。

## 🌐 公開URL

- **本番（常に最新）**: https://favorite-recipes-mu.vercel.app/
- **デプロイ先URL（固定）**: https://favorite-recipes-8symmq9cf-yukihsuns-projects.vercel.app

> 本番エイリアス（`*-mu.vercel.app`）は常に最新デプロイを指すのに対し、
> 2つ目のURLは今回のビルドに固定された deployment-specific URL です。

## 機能

- レシピ5件を材料・作り方付きで掲載（鶏のからあげ／豚の生姜焼き／ほうれん草のお浸し／ミートソースパスタ／バスクチーズケーキ）
- キーワード検索（レシピ名・材料）
- カテゴリ絞り込み（メイン／副菜／スイーツ）
- お気に入りトグル（LocalStorageに保存）

## 技術スタック

- HTML / CSS / JavaScript を1ファイル (`index.html`) に同梱
- ホスティング: [Vercel](https://vercel.com)
- CI/CD: Vercel CLI 経由でのデプロイ（将来的に GitHub → Vercel の Push-to-Deploy に移行予定）

## ローカルで見る

```bash
open index.html
```

## デプロイ

Vercel CLI から本番デプロイしています。

```bash
export VERCEL_TOKEN='vcp_xxxxxxxxxxxxxxxx'
vercel deploy --prod --yes --token "$VERCEL_TOKEN" --scope yukihsuns-projects
```

### ⚠️ トークン有効期限

本プロジェクトで使用中の Vercel Personal Access Token は
**2026-06-18 (June 18, 2026)** に失効します。
それ以降、CLI から再デプロイする場合は新しいトークンを発行して
`VERCEL_TOKEN` を更新してください。

> サイト自体はトークン失効後もそのまま動作し続けます。
> 失効するのは「CLI から再デプロイする権限」のみです。
