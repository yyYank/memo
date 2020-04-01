---
title: "Dockerメモ"
date: 2020-04-01T15:57:47+09:00
draft: false
weight: 100
---

## 容量確認

```
docker system df
```

## 色々消す

```
docker system prune -a --volumes
```

## コンテナ消す

```
docker container prune
```

## イメージ消す

```
docker image prune
```

## ボリューム消す

```
docker volume prune
```

## 起動しているコンテナ一覧

```
docker ps
```

## コンテナ一覧

```
docker ps -a
```

## イメージ一覧

```
docker images
```

## イメージ指定して削除

```shell
docker rmi [ImageID]
```
