---
title: "gitメモ"
date: 2020-04-01T16:02:44+09:00
draft: false
weight: 100
---

## developとmasterにマージ済みのローカルブランチを削除する

```
git branch --merged|egrep -v '\*|develop|master'|xargs git branch -d
```

## authorをammendしたいとき

```
git commit --amend --author="name <hoge@gmail.com>"
```
