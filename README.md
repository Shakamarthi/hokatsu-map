# 保活管理システム v2.5

## 今回の変更

- 園カード上部に重要条件をアイコン表示
  - 区分
  - 通園負荷
  - 延長保育（0歳児利用可否＋終了時刻）
  - 用品サブスク
  - おむつ
  - 園庭
  - 入園難易度
  - 評価
- 「園の詳細を見る」を追加
- 延長保育を単純な有無ではなく条件付きデータとして管理
- 公式HPリンク欄を追加
- 公式URL未登録の園は「公式HP検索」を表示
- Googleマップ／Appleマップリンクを維持

## GitHub更新対象

以下の2ファイルをリポジトリ直下へ上書きしてください。

- `index.html`
- `hokatsu-data.json`

`README.md` はGitHubへ置かなくても動作します。

## データ入力方針

未確認情報は推測で埋めず、「要確認」としています。
見学資料や公式HPで確認できた園から、`hokatsu-data.json` の以下を更新してください。

- `officialUrl`
- `quickFacts`
- `details`

## 延長保育の主要項目

- `available`
- `infantAvailable`
- `minimumAge`
- `standardEnd`
- `extendedEnd`
- `usageType`
- `snack`
- `dinner`
- `note`
