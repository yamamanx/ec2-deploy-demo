# EC2 Deploy Demo

AWS CodeDeployを使用してEC2インスタンスにWebアプリケーションをデプロイするサンプルプロジェクトです。

## ファイル構成

```
├── index.html          # Version 1 (薄い青色の背景)
├── update.html         # Version 2 (薄いグリーンの背景)
├── appspec.yml         # CodeDeploy設定ファイル
├── scripts/
│   ├── install_nginx.sh # NGINXインストール
│   ├── stop_server.sh   # サーバー停止
│   └── start_server.sh  # サーバー開始
└── .gitignore
```

## デプロイ手順

1. EC2インスタンスにCodeDeploy Agentをインストール
2. このリポジトリをGitHubまたはS3にアップロード
3. CodeDeployアプリケーションとデプロイメントグループを作成
4. デプロイメントを実行

## バージョン更新

Version 2にアップデートする場合は、`index.html`を`update.html`の内容で置き換えてデプロイしてください。