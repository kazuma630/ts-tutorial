## セットアップ
```
// リポジトリをクローン
git clone https://github.com/kazuma630/ts-tutorial.git

// プロジェクトディレクトリへ移動
cd ts-tutorial

// dockerコンテナをビルド → バックグラウンド実行
docker compose up -d --build

// nodeコンテナの中に入る
docker compose exec node-dev sh

// package.jsonの情報をもとに、typescriptインストール
npm install

// tsファイルをjsファイルにコンパイル
npx tsc

// コンパイルされたjsファイルをnodeで実行
node dist/index.js

「hello world!」が表示されていれば、成功！
```