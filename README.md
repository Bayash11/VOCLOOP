# VOCLOOP v1.0 (initial build)

個人用の英単語反復学習アプリ。静的HTML/CSS/JavaScript、IndexedDB、Service Workerを使用します。

## 実行
HTTPSの静的ホスティング（例：GitHub Pages）にファイルを置いて `index.html` を開いてください。`file://` ではService Workerが動作しません。

## 重要
- 学習データは利用端末のブラウザに保存され、GitHubにアップロードされません。
- 設定から定期的にJSONバックアップを保存してください。
- JSON単語登録は `words` 配列の各要素に `term`, `meaning`, `katakana`, `stress`, `pos`, `example`, `translation`, `usage`, `priority` を指定します。
- 学習ロジック・復元・オフライン動作は実機での追加検証が必要です。