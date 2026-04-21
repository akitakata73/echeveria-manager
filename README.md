# エケベリア管理 PWA v30 Last Recovery

## v30の目的

v25・v26・v27系の保存データを、最後の復旧候補として設定画面に表示する版です。

## 重要

- 起動時に旧データを自動採用しません。
- 通常保存キーは `echeveria_pwa_data` のままです。
- 設定画面の「保存データ診断・復旧候補」から、必要なデータだけ手動採用できます。
- 採用前には緊急バックアップを自動作成します。

## 表示対象

- echeveria_pwa_data
- echeveria_pwa_v30_last_recovery_data
- echeveria_pwa_v29_stable_data
- echeveria_pwa_v28_target_recovery_data
- echeveria_pwa_v27_manual_recovery_data
- echeveria_pwa_v27_data
- echeveria_pwa_v26_stable_data
- echeveria_pwa_v26_data
- echeveria_pwa_v25_recovery_data
- echeveria_pwa_v25_data

## 確認手順

1. `?v=30-last-recovery` で開く
2. 設定画面を開く
3. 復旧候補の株数・履歴数・写真数・最新日時を確認
4. 必要な候補があれば「このデータを採用」
5. 採用後、株一覧・履歴を確認
6. 正しければJSONバックアップを取得
