# ClarTone — 法務ページ（公開用）

iOS アプリ「ClarTone - クラリネット音出し練習」の**サポート・法務ページのみ**を GitHub Pages で公開するリポジトリです。

アプリ本体は Private のままにし、本リポジトリだけ Public にします。

## 公開 URL

ベース: `https://funakitakuya.github.io/ClarTone-Legal/`

| ページ | URL |
|--------|-----|
| トップ（一覧） | `…/` または `…/index` |
| 使い方ガイド | `…/guide` |
| User Guide (EN) | `…/guide-en` |
| サポート | `…/support` |
| プライバシーポリシー | `…/privacy-policy` |
| 利用規約 | `…/terms-of-use` |
| 特定商取引法に基づく表記 | `…/tokushoho` |

アプリ内の `ToneLegalURLs.baseURLString` は次と一致させます。

`https://funakitakuya.github.io/ClarTone-Legal`

## 初回セットアップ（GitHub）

1. GitHub で **Public** リポジトリ `ClarTone-Legal` を作成
2. ローカルから push:

```bash
cd "/Users/takuya/iPhoneApp/ClarTone-Legal"
git init
git remote add origin https://github.com/FunakiTakuya/ClarTone-Legal.git
git branch -M main
git add -A && git commit -m "Initial ClarTone legal pages"
git push -u origin main
```

3. **Settings → Pages** → Branch: `main`、Folder: **`/ (root)`** → Save
4. 1〜3 分後、上記 URL がブラウザで開けることを確認

## 文言の更新

正本は Private リポジトリ `iOS_app/ClarTone` の `Legal/` です。

```bash
cd "/Users/takuya/iPhoneApp/iOS_app/ClarTone"
./scripts/sync-legal-to-public-repo.sh
cd "/Users/takuya/iPhoneApp/ClarTone-Legal"
git add -A && git commit -m "Update legal pages" && git push
```

## ファイル構成

- `index.md` — ページ一覧
- `guide.md` / `guide-en.md` / `support.md` / `privacy-policy.md` / `terms-of-use.md` / `tokushoho.md`
- `_config.yml` — GitHub Pages（Jekyll）設定（sync で上書きされない）
