# エケベリア管理 PWA v48 Watering Connection Fix

## 主な変更点
- openWater 冒頭で株存在確認を追加
- 通常水やり画面の保存ボタンを saveWater('${pid}') に修正
- saveWater(pid) は pid 未指定時に selectedPlantId を補完
- 保存方式全体には触れず、通常水やりの接続不良のみを局所修正
