保活管理システム v2.2（GitHub JSON正本版）

【正本】
GitHubリポジトリ直下の hokatsu-data.json

【GitHub Pagesへの反映】
以下の2ファイルをリポジトリ直下へアップロードしてください。
- index.html
- hokatsu-data.json

【運用】
1. Webアプリ起動時に hokatsu-data.json を読み込みます。
2. 画面変更は端末下書きとして自動保存されます。
3. 確定時は「正本更新用JSON」を押します。
4. ダウンロードされた hokatsu-data.json でGitHub上の同名ファイルを置き換えます。
5. Pages反映後「GitHub正本を再読込」を押します。

【重要な制約】
GitHub Pagesは静的サイトのため、ブラウザからリポジトリへ安全に直接書き込めません。
Personal Access TokenをHTMLへ保存する方式は漏えいリスクがあるため採用していません。
そのため「入力→JSON書き出し→GitHubで置換」を安全な確定手順としています。

【端末間利用】
- GitHub反映済み正本はiPhone・PC・Safari・Edgeで共通です。
- GitHub未反映の下書きは端末・ブラウザごとに別です。

【確認URL】
https://shakamarthi.github.io/hokatsu-map/?v=2.2
