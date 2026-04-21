# エケベリア管理 PWA v35 Data Guard

## v35の目的
v34で空データでは起動できる一方、実データの一部欠損により表示が止まる可能性があったため、読込時のデータ補正を強化した版です。

## 主な修正
- masters.cultivars / pots / media / trays が欠けていても既定値で補完
- plants / histories / photos が配列でない場合も安全に補正
- 履歴日時が欠けていてもホーム画面の並び替えで落ちないよう修正
- mList / mName / activePlants を安全化
- 株名・ID・状態などの最低限の既定値を補完
- 実行時エラーが起きた場合、真っ白ではなくエラー表示を出す

## 保存方式
- 固定キー：echeveria_pwa_data
- 直前データ：echeveria_pwa_previous_data
