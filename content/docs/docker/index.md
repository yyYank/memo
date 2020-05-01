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

## dockerの諸々の場所(linux)

```
/var/lib/docker
```

## docker関連でよく使うコマンド


ログ見る

```
docker logs -f hoge
```

再起動

```
docker restart hoge
```

起動

```
docker start hoge
```

bashでもぐる


```
docker exec -it hoge /bin/bash
```

## Linux + postgresコンテナをシュッと作ってGoのプロジェクトのユニットテスト

```
docker run --privileged --name centos -d centos /sbin/init
docker exec -ti centos bash
yum install -y git
yum install -y epel-release
yum install -y golang
yum install -y https://yum.postgresql.org/9.6/redhat/rhel-7-x86_64/pgdg-redhat96-9.6-3.noarch.rpm
yum install -y postgresql96-server postgresql96-contrib
PGDATA=/var/lib/pgsql/data /usr/pgsql-9.6/bin/postgresql96-setup initdb
systemctl start postgresql-9.6.service
git clone [repo url]
cd [repo]
go test ./..
```
