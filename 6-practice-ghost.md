# 6. Ghost

## 6.1 firewalld のポート公開 (RHEL7の場合)

```
firewall-cmd --add-service=http --permanent
firewall-cmd --reload
```

## 6.2 Ghost セットアップ

```
docker run  -p 80:2368 -d ghost
```

## 6.3 コンテナ ID の確認

```
docker ps
```

## 6.4 コンテナの停止

```
docker stop <コンテナID>
```
 
[次へ](7-practice-wordpress.md)

