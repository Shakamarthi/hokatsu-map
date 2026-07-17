# 保活管理システム v2.7.4

## 修正内容

v2.7.2〜v2.7.3で発生したGoogleマイマップ閲覧動作の回帰を修正しました。

- 閲覧URLをv2.7.1で使用していた形式へ戻しました
  - `https://www.google.com/maps/d/viewer?hl=ja&mid=...`
- 閲覧リンクの属性もv2.7.1と同じ構成へ戻しました
- 編集URLは以下を維持します
  - `https://www.google.com/maps/d/edit?mid=...&ll=35.66216420142517%2C139.85870817502527&z=15`
- PWAキャッシュを `hokatsu-map-v274` に更新

## GitHubへ上書きするファイル

- `index.html`
- `sw.js`
- `manifest.webmanifest`

`hokatsu-data.json` は変更していません。

## 初回確認URL

https://shakamarthi.github.io/hokatsu-map/?upgrade=274
