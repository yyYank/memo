---
title: "vimメモ"
date: 2020-04-01T16:02:47+09:00
draft: false
weight: 100
---

# Vim

## ファイルパスジャンプ

```
gf
```

gfはgoto fileの略

## vsplitしてファイルパスジャンプ

```
<C-w>f
```

## tabsplitしてファイルパスジャンプ

```
CTRL-W gf 
```

## ファイルジャンプ系プラグイン

https://github.com/kana/vim-altr

## ソートして重複消す

```
sort u
```

## たまに使いたくなる

```
smile
```

# NERDTREE

## ウインドウサイズ調整

```
let g:NERDTreeWinSize=40
:NERDTree
```

`:NERDTreeFind` ,とかだとWindowサイズがリセットされない。数字は任意
                     
## 現在開いてるファイルの位置表示

```
NERDTreeFind
```
                     

