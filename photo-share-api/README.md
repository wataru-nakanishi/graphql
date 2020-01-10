# graphql-server
## mongodb環境構築
1. docker hubからイメージ取得
```
docker pull mongo
```
2. docker-compose.yml作成

3. コンテナへアクセス
```
docker-compose exec mongo bash
mongo admin -u root -p <YOUR PASSWORD>
```



### .env作成
```
DB_HOST=mongodb://root:example@127.0.0.1:27017/admin
CLIENT_ID=<YOUR_GITHUB_CLIENT_ID>
CLIENT_SECRET=<YOUR_GITHUB_CLIENT_SECRET>
```

### 参考
https://hub.docker.com/_/mongo/
https://qiita.com/mistolteen/items/ce38db7981cc2fe7821a
