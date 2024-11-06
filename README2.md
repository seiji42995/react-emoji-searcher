## 注意点
root直下に存在するpackage.jsonの6行目の表記は開発時のみ有効な設定となっています。セキュリティの観点より運用は想定していません。
（変更前）"dev": "next dev"
（変更後）"dev": "NODE_TLS_REJECT_UNAUTHORIZED=0 next dev"

## 動作確認時に必要な設定
・API用サーバの用意
以下URL先のREADME記載の「Server startup」の作業を実施し、サーバを用意し起動。
https://github.com/cheatsnake/emojihub?tab=readme-ov-file#readme
