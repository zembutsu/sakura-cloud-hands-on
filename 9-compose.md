#9. Docker Compose

9.1. Docker Compose をセットアップ

```
curl -L https://github.com/docker/compose/releases/download/1.8.0/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```

9.2. インストールを確認

```
docker-compose  version
```

9.3. [docker-compose.yaml](./rocketchat/docker-dompose.yaml) の作成

```
git clone \ https://github.com/zembutsu/sakura-cloud-hands-on.git
cd sakura-cloud-hands-on/rocketchat
```

9.4. イメージの取得

```
docker-compose pull
```

9.5. イメージを確認

```
docker images
```

9.6. compose で複数のコンテナを起動

```
docker-compose up -d
```

9.7. コンテナを確認

```
docker ps
```

9.8. firewalld で通信を許可

```
firewall-cmd --add-port=3000/tcp --zone=public --permanent
firewall-cmd --reload
```

9.10 ブラウザで ``http://<ip>:3000`` を確認

[目次](README.md)



