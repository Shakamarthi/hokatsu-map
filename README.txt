保活管理システム v2.3（GitHub API直接保存版）

【構成】
- index.html
- hokatsu-data.json

【修正内容】
- v2.2のJavaScript構文不具合を修正
- GitHub Contents APIから正本を読み込み
- Webアプリから hokatsu-data.json を直接更新
- 更新競合（HTTP 409）を検出
- トークンをsessionStorageのみに保持
- 端末下書きはlocalStorageへ自動保存

【GitHubトークンの作成】
GitHub Settings → Developer settings → Personal access tokens → Fine-grained tokens

推奨設定：
- Expiration：必要最小限
- Repository access：Only select repositories
- 対象：shakamarthi/hokatsu-map
- Repository permissions → Contents：Read and write
- その他の権限：原則 No access

トークンはWebアプリの入力欄へ入力します。
HTMLやhokatsu-data.jsonには書き込まれませんが、ブラウザで動く仕組みである以上、
第三者端末や共有端末では入力しないでください。

【GitHubへの反映】
リポジトリ直下の以下2ファイルを置き換えてください。
- index.html
- hokatsu-data.json

【公開確認URL】
https://shakamarthi.github.io/hokatsu-map/?v=2.3
