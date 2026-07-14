GitHub Pages 差し替え手順

1. このフォルダ内の index.html を、GitHubリポジトリ直下の既存 index.html と置き換える。
2. manifest.webmanifest と sw.js は削除して構いません。v5はサービスワーカーを使いません。
3. Commit changes を押す。
4. 1〜3分待ち、Safariで以下を開く。
   https://shakamarthi.github.io/hokatsu-map/?v=5
5. 古い表示が残る場合はSafariでページを再読み込み。必要なら設定→Safari→詳細→Webサイトデータから github.io を削除。

v5の変更点
- Safariで失敗していたfetch/CORS方式を廃止
- JSONP方式で住所照合
- 旧サービスワーカーを自動解除
- キャッシュ抑止
