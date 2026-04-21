# エケベリア管理 PWA v41 Photo Stability

## v41の目的

v39〜v40でIndexedDBへ切り離した写真運用を安定化する版です。

## 主な変更点

- 写真本体が見つからない場合に「写真本体なし」と表示
- 壊れた画像や空白表示を避ける
- 写真追加時は、IndexedDBへの写真本体保存成功後にだけメタ情報を追加
- IndexedDB保存に失敗した場合、写真メタ情報も追加しない
- 写真追加失敗時は「写真の保存に失敗しました。写真は追加されていません」と表示
- 写真メタ情報枚数と未移行写真数を設定画面で表示
- v40 Safe Commit の保存確定処理は維持

## 維持している固定ルール

- 保存キー：echeveria_pwa_data
- 直前データ：echeveria_pwa_previous_data
- 写真本体：IndexedDB
- 旧キー自動採用なし
- 保存データ診断・復旧候補欄なし
- localStorage.clear() 未使用
