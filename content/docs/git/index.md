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

## gitのremote urlをhttpsからsshに変更したい

```
git remote set-url origin git@github.com:{repository_owner}/{repository_name}.git
```

## git rebaseのなんだっけ？メモ

### d, drop


```
remove commit
ドロップ=コミットを削除
```

### x, exec

```
exec = run command (the rest of the line) using shel
x、exec =シェルを使用してコマンド（行の残りの部分）を実行
```

### f, fixup

```
like "squash", but discard this commit's log message
「スカッシュ」のようですが、このコミットのログメッセージを破棄します
```

### s, squash

```
use commit, but meld into previous commit
コミットを使用しますが、以前のコミットにマージします
```

### e, edit

```
use commit, but stop for amending
コミットを使用しますが、修正のために停止します
```

### r, reword

```
use commit, but edit the commit message
コミットを使用しますが、コミットメッセージを編集します
```

