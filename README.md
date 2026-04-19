# エケベリア管理 PWA v2

## 変更点
- 新規株登録時に「＋品種を新規追加」を選べるように変更
- 登録時に「お迎え日」を入力できるように変更
- 登録時に「最終水やり日・量・mL・方法」を別枠で入力可能に変更
- 次回確認日の自動提案を追加
- ホーム画面内通知として「期限超過」「本日確認」の件数を表示
- v1のlocalStorageデータを自動移行

## 更新方法
GitHubのリポジトリで以下を上書きしてください。

- index.html
- manifest.webmanifest
- service-worker.js
- icon-192.png
- icon-512.png
- README.md

更新後、GitHub PagesのURLをSafariで再読み込みしてください。
ホーム画面アプリ側で古い表示が残る場合は、SafariでURLを開いて更新し直してください。
