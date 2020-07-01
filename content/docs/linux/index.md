---
title: "Linuxメモ"
date: 2020-04-22T14:43:05+09:00
draft: true
---


想定としてはubuntu、archなど。コマンドはmacでも使えるかも


## port使っているやつを見つける

```
lsof -n -P -i:8981
```


## とりあえず色々見たい

```
journalctl -f
```

## サービス動かしたい


```
systemctl start hoge
systemctl stop hoge
systemctl restart hoge
```

## サービスの状況を見たい

```
systemctl status hoge
```

### apt-getのあれ

```
apt-get install hoge
apt-get remove hoge
```
