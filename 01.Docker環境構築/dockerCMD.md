1. MySQLのDockerImageをプル
```
docker pull mysql
```

2. Dockerコンテナを起動
```
docker run --name io-mysql -p 13306:3306 -e MYSQL_ROOT_PASSWORD=!QAZ2wsx -d mysql
```

3. Dockerコンテナの中に入る
```
docker exec -it io-mysql bash
```

4. Dockerコンテナを停止させる
```
docker stop io-mysql
```

5. 一度停止させたコンテナを再度起動する
※docker run:コンテナイメージからコンテナを作成して起動 docker start: 構築して停止したコンテナを起動