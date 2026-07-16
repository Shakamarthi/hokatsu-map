# 保活管理システム v2.6.1

## 今回の修正

v2.4の画面が残り続けた原因となる旧Service Workerキャッシュを更新します。

- キャッシュ名を `hokatsu-map-v261` に更新
- 旧キャッシュをactivate時に自動削除
- `index.html` と `hokatsu-data.json` をネットワーク優先に変更
- 新Service Workerを即時有効化
- manifestを現行アプリ名へ更新
- iPhoneホーム画面追加に必要なPWA設定を追加

## GitHubへ上書きするファイル

今回は次の3ファイルを必ず上書きしてください。

- `index.html`
- `sw.js`
- `manifest.webmanifest`

`hokatsu-data.json` は変更していません。

## 反映後

1. GitHub Pagesのデプロイ完了を待つ
2. 次のURLをブラウザで開く  
   https://shakamarthi.github.io/hokatsu-map/?upgrade=261
3. 1回開いた後、必要ならホーム画面の旧アイコンを削除して再追加する

通常は新Service Workerが旧キャッシュを削除するため、ブラウザを変える必要はありません。
