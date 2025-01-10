# ![ヘッダー画像](assets/header.svg)

## 📖 プロジェクト目的
このプロジェクトはWindows環境でcode-serverをDockerコンテナとして簡単に実行するための最小構成を提供します。

## 🛠 使用方法

<div align="center">
  <img src="https://github.com/user-attachments/assets/33648eb0-f86e-4e45-a072-3cc6d5946ea4" alt="GitHubバッチ" />
  <img src="https://github.com/user-attachments/assets/33648eb0-f86e-4e45-a072-3cc6d5946ea4" alt="技術スタックバッチ" />
</div>

1. 環境変数の設定
   - `.env`ファイルに以下の内容を記載：
     ```
     USERPROFILE=${env:USERPROFILE}
     USERNAME=${env:USERNAME}
     ```

2. Docker Composeの実行
   ```powershell
   docker-compose up
   ```

3. code-serverのアクセス
   - ブラウザで `http://127.0.0.1:8080` にアクセス

## ⚠ 注意点
- Docker Desktop for Windowsがインストールされていることを確認してください
- すでに `code-server` というコンテナが存在する場合は、先に削除する必要があります：
  ```powershell
  docker rm code-server
  ```
- 初回実行時はコンテナイメージのダウンロードに時間がかかる場合があります

## 🌱 環境変数
| 変数名 | 説明 |
| --- | --- |
| USERPROFILE | Windowsのユーザープロファイルディレクトリ |
| USERNAME | Windowsのユーザー名 |

## 🎨 SVGヘッダー画像
![ヘッダー画像](assets/header.svg)
