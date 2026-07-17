# 保活管理システム v2.8.1

## 主な変更

- 画面右上に「⚙️ 設定」を追加
- GitHub設定を `hokatsu-settings` として端末内に永続保存
- バージョンアップ後も同じブラウザ・同じサイトであれば再入力不要
- 設定画面から以下を変更可能
  - Owner
  - Repository
  - Branch
  - データファイル
  - Personal Access Token
  - Googleマイマップ閲覧URL
  - Googleマイマップ編集URL
- トークンは通常伏字で表示
- トークン削除、端末下書き削除、GitHub再読込を設定画面に集約
- 旧sessionStorageのトークンが残っている場合は自動移行
- PWAキャッシュを `hokatsu-map-v281` に更新

## セキュリティ

トークンはGitHub Pagesのファイルや `hokatsu-data.json` には保存されません。
この端末のブラウザのlocalStorageに保存されます。

ただし、端末を共有している場合やブラウザのサイトデータを削除した場合は、再設定が必要です。

## GitHubへ上書きするファイル

- `index.html`
- `sw.js`
- `manifest.webmanifest`

`hokatsu-data.json` は変更していません。

## 初回確認URL

https://shakamarthi.github.io/hokatsu-map/?upgrade=281
