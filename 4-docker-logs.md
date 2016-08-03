## 4. ログの表示

4.1. ログ表示コマンド

```
docker logs <コンテナID>
```

4.2. 最後の3行を表示

```
docker logs -tail 3 <コンテナID>
```

4.3. ログを表示し続ける

```
docker logs --tail 1 --follow <コンテナのID>
```

[次へ](5-docker-stop.md)

