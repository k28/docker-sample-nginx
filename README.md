# NginxサーバをDockerで立ち上げるサンプル

テスト的にhtmlサーバをサクッと立ち上げたい使う。

## ポート番号
8080ポートにhttpで接続可能

## ファイル構成

```
├── README.md
├── docker-compose.yml
├── nginx
│   ├── Dockerfile
│   └── nginx.conf
└── public                  <= HTMLファイルを置く
    └── index.html
```

## 立ち上げ方
```
$ docker-compose up -d
```

```
http://localhost:8080/
```
でindex.htmlが表示される

## 使わなくなったら...
```
$ docker-compose down
```

