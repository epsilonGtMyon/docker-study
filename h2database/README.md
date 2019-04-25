# h2データベース用のコンテナ
とりあえず作ってみた


## 動かす
```
docker build -t h2-sandbox .

docker run -d -p 80:8082 -p 9092:9092 h2-sandbox
```