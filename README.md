# Laravel テンプレ
クローン
`git clone https://github.com/Gin58/Plane.git`

planeフォルダの名前を任意に

## 修正要
`docker-compose.yml`
```
container_name(web,app,db)
volumes(web,app)
workign_dir(app)
```

`Dockerfile`
```
LABEL maintainer "好きなのに変更"
```

`docker/nginx/default.conf`
```
root /好きなのに/public
```

`.env`
```
DB_NAME=好きなのに
```

# 変更終了後
ビルドする
`docker-compose build`

立ち上げる
`docker-compose up`

# Laravel インストール
appコンテナに入る
`docker-compose exec app ash`

プロジェクト作成
`composer create-project --prefer-dist "laravel/laravel=6.0.*" .`

バージョン確認
`php artisan -V`

最初の画面確認
localhost:8080にアクセス
