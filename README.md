# Favorite Recipes

お気に入りレシピを管理する静的Webサイト。
単一のHTMLファイル（HTML / CSS / JavaScript）で構成され、Vercel で公開しています。

## 機能

- レシピ5件を材料・作り方付きで掲載（鶏のからあげ／豚の生姜焼き／ほうれん草のお浸し／ミートソースパスタ／バスクチーズケーキ）
- キーワード検索（レシピ名・材料）
- カテゴリ絞り込み（メイン／副菜／スイーツ）
- お気に入りトグル（LocalStorageに保存）

## 技術スタック

- HTML / CSS / JavaScript を1ファイル (`index.html`) に同梱
- ホスティング: [Vercel](https://vercel.com)
- CI/CD: GitHub → Vercel の Push-to-Deploy

## ローカルで見る

```bash
open index.html
```

## デプロイ

`main` ブランチに push すると、Vercel が Webhook を検知して自動ビルド＆デプロイされます。
