# 保活管理システム v2.7.1

## 今回の変更

- トップ画面の「データ品質」パネルを削除
- 園カード上の「データ充足率」表示を削除
- 詳細画面から未確認件数・充足率を削除
- 情報源と最終精査日は詳細画面に維持
- `hokatsu-data.json` 内の `dataQuality` は保守・データ精査用として維持
- PWAキャッシュを `hokatsu-map-v271` に更新

## 設計方針

データ品質管理は必要ですが、日常の保活活動で常時見る情報ではありません。
そのため、利用者向けUIからは外し、JSON内部の管理情報として保持します。

## GitHubへ上書きするファイル

今回はUI変更のため、次の3ファイルを上書きしてください。

- `index.html`
- `sw.js`
- `manifest.webmanifest`

`hokatsu-data.json` はv2.7から変更していません。

## 初回確認URL

https://shakamarthi.github.io/hokatsu-map/?upgrade=271
