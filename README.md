# エケベリア管理 PWA v34 Runtime Fix

## v34の目的

v33で画面が表示されなくなった実行時エラーを修正した版です。

## 原因

v33の末尾付近に、不要な `async` だけが単独で残っていました。

```js
async

function openImport(){...}
```

これは構文チェックでは通る一方、実行時に未定義変数 `async` として評価され、そこでJavaScriptが停止します。
その結果、`load(); go("home");` まで到達せず、画面が表示されませんでした。

## 修正内容

- 単独で残った `async` を削除
- v33の保存状態表示は維持
- 保存サイズ表示、写真枚数表示、最終保存成功時刻表示も維持
- 固定キー＋直前データ方式を維持

## 保存方式

- 固定キー：echeveria_pwa_data
- 直前データ：echeveria_pwa_previous_data
