# エケベリア管理 PWA v32 Safe Save

## v32の目的

v31の「写真込みデータを多世代に保存しすぎる」問題を修正し、シンプルで安全な保存方式に変更した版です。

## 主な変更点

- 旧復旧候補欄を削除
- 保存キーは固定 `echeveria_pwa_data`
- 保存先は固定キー + previous の2系統に限定
  - echeveria_pwa_data
  - echeveria_pwa_previous_data
- 多世代ミラー保存を廃止
- 起動時に勝手に保存しない
- 固定キーが壊れている場合のみ previous を読み込む
- 保存成功／保存失敗を設定画面に表示
- 保存失敗時は強い警告を表示
- pagehide / visibilitychange で保存を試行
- クローン作成・中株・基準日数見直しを再統合

## 注意

SafariのWebサイトデータ削除を行うと、fixed / previous / emergency すべて消える可能性があります。
重要な節目ではJSONバックアップも併用してください。
