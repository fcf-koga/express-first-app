<!-- シールド一覧 -->
<!-- 該当するプロジェクトの中から任意のものを選ぶ-->
<p style="display: inline">
  <!-- フロントエンドのフレームワーク一覧 -->
  <img src="https://img.shields.io/badge/-Node.js-000000.svg?logo=node.js&style=for-the-badge">
  <img src="https://img.shields.io/badge/-Express.js-000000.svg?logo=express.js&style=for-the-badge">
  <img src="https://img.shields.io/badge/-MongoDB-000000.svg?logo=mongodb&style=for-the-badge">
</p>

# express-first-app
Express.jsのMDNチュートリアルで作成したアプリケーション

https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs

## バージョン
```
node -v
v20.14.0

npm -v
10.7.0
```


## 実行方法
```
cd express-first-app

npm install

DEBUG=express-first-app:* npm start

//nodemon
DEBUG=express-first-app:* npm run devstart

```

## MongoDBの起動
```
docker compose up -d
```

### MongoDBへの接続
```
docker compose exec mongo bash

mongosh --port 27017  --authenticationDatabase -u "root" -p

Enter password:
<!-- パスワードはdocker-compose.ymlで設定したもの -->
```

### サンプルデータのインポート
```
node populatedb mongodb://root:example@localhost:27017

```

## アクセスURL
http://localhost:3000/
