# 保活管理システム v2.7

## 目的

v2.1以降に追加してきたデータ項目を整理し、`hokatsu-data.json`を長期運用可能な正本へ再設計しました。

## 主な変更

- JSONを以下の責務単位に正規化
  - `basic`
  - `official`
  - `commute`
  - `services`
  - `operations`
  - `admissionDifficulty`
  - `evaluation`
  - `dataQuality`
- `要確認`という文字列を正本データから削除
  - 未確認値は原則 `null`
  - 画面表示時にだけ「要確認」と表示
- 園ごとに以下を自動管理
  - データ充足率
  - 未確認項目一覧
  - 最終精査日
  - 情報源
- 旧形式JSONの読み込み互換性を維持
- JSON書き出し・GitHub保存はv2.7形式に統一
- PWAキャッシュを `hokatsu-map-v27` に更新

## GitHubへ上書きするファイル

- `index.html`
- `hokatsu-data.json`
- `sw.js`
- `manifest.webmanifest`

## 初回確認URL

https://shakamarthi.github.io/hokatsu-map/?upgrade=27

## 補足

本版はデータ構造の整理を主目的としています。
「未確認項目がゼロ」という意味ではなく、確認済み情報と未確認情報を明確に分離し、残件を可視化する版です。
