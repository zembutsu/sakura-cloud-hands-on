#7. WordPress と MySQL コンテナ

7.1. WordPress の実行

```
docker run wordpress
```

7.2. mysql イメージのダウンロード

```
docker pull mysql
```
 
7.3. MySQL の設定
 
 ```
 docker run --name mysql -e MYSQL_ROOT_PASSWORD=パスワード -d mysql
 ```
 
7.4. WordPress の立ち上げ
 
 ```
 docker run --name wordpress --link mysql:mysql -p 80:80 wordpress
```

* Ctrl + C で中断

7.5 バックグラウンドで実行

```
docker run --name wordpress2 -d --link mysql:mysql -p 80:80 wordpress
```

7.6 停止

```
docker kill <コンテナID>
```

 
 
[次へ](8-dockerfile.md)

