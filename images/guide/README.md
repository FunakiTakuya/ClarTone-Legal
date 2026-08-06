# ガイド画像

App Store 提出用スクショ（`AppStoreAssets/Screenshots-6.7/Upload-ASC-6.5/`）から Web 用に縮小した JPEG です（幅 **180px**・FluteTone ガイドと同寸）。

| ファイル | 内容 |
|----------|------|
| `ja/01-home.jpg` / `en/01-home.jpg` | ホーム |
| `ja/02-practice.jpg` / `en/02-practice.jpg` | 練習中 |
| `ja/03-review.jpg` / `en/03-review.jpg` | 振り返り |
| `ja/04-pro.jpg` / `en/04-pro.jpg` | Pro 購入 |

`guide.md` / `guide-en.md` から相対パス `images/guide/...` で参照します。  
差し替え時は ASC フォルダを更新したうえで再縮小し、`scripts/sync-legal-to-public-repo.sh` で `docs/`（と公開リポ下書き）へ同期してください。
