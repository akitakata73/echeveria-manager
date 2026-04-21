# エケベリア管理 PWA v28 Target Recovery

## v28の目的

今回の復旧作業用に、保存データ診断の対象を絞った版です。

## 変更点

- 診断表示対象を以下に限定
  - echeveria_pwa_data
  - echeveria_pwa_v28_target_recovery_data
  - echeveria_pwa_v27_manual_recovery_data
  - echeveria_pwa_v26_stable_data
  - echeveria_pwa_v26_data
  - echeveria_pwa_v25_recovery_data
  - echeveria_pwa_v25_data
- v19〜v24の旧キー群は診断表示から除外
- 起動時に旧キーを自動採用しない
- 必要なキーだけ、設定画面から手動で「このデータを採用」する方式

## 注意

この版は復旧対象を絞るための一時版です。
正しいデータを採用できたら、すぐJSONバックアップを取得してください。
