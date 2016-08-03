#8. Dockerfile

8.1. ディレクトリの作成と移動

```
mkdir myimage
cd myimage
```


8.2. エディタで Dockerfile を作成

```
vim Dockerfile
```

ファイル内容は

```
FROM ubuntu
RUN apt-get update
RUN apt-get install -y wget
```

* ``a`` を入力してモード変換
* 終了は ``ESC`` キーを一度押してから ``:wq`` エンターを入力

あるいは、以下のコマンドを実行

```
cat << EOF > ./Dockerfile
FROM ubuntu
RUN apt-get update
RUN apt-get install -y wget
EOF
```

8.3. ``myimage`` イメージをビルド

```
docker build -t myimage .
```

8.4 コンテナの実行

```
docker run -it myimage bash
```
 
[次へ](9-compose.md)

