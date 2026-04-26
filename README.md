# エケベリア管理 PWA v49 Observe Safe Fix

## 主な変更点
- 通常観察の入力を専用正規化処理へ変更
- 次回確認日は専用の安全計算関数で算出
- YYYY-MM-DD 形式検証を追加
- openObserve 冒頭で株存在確認を追加
- 観察画面の保存ボタンを saveObserve('${pid}') に修正
- saveObserve(pid) は pid 未指定時に selectedPlantId を補完
- 検証成功までは株本体を書き換えない
- save() 失敗時は対象株をロールバック
- エラー時は「保存していません」と明示
- 保存方式全体には触れず、通常観察処理のみを局所修正
