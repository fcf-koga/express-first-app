# express-first-app
Express.jsのMDNチュートリアルで作成したアプリケーション

# バージョン
```
node -v
v20.14.0

npm -v
10.7.0

# 実行方法
```
cd express-first-app
npm install
DEBUG=express-first-app:* npm start
//nodemon
DEBUG=express-first-app:* npm run devstart

```

# MongoDBの起動
```
docker compose up -d

## MongoDBへの接続
docker compose exec mongo bash

mongosh --port 27017  --authenticationDatabase -u "root" -p
Enter password:
<!-- パスワードはdocker-compose.ymlで設定したもの -->

## サンプルデータのインポート
node populatedb mongodb://root:example@localhost:27017

```

http://localhost:3000/
