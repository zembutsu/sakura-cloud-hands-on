## 2. コンテナの起動

2.1. Hello World

```
docker run hello-world
```

2.2. ubuntu を実行

```
docker run -it ubuntu bash
```

2.3. ``curl`` のインストール

```
apt-get update
apt-get install curl
```

2.4. ``curl`` コマンドの確認

```
curl ifconfig.me/ip
```

2.5. コンテナを終了

```
exit
```

2.6. 再度コンテナを実行

```
docker run -it ubuntu bash
curl ifconfig.me/ip
```

[次へ](3-background.md)
