---
title: "npm vs yarnメモ"
date: 2020-04-26T00:24:25+09:00
draft: true
---


## プロジェクト作成

### npm
 
```
npm init
```

### yarn

```
yarn init
```

## typescript依存追加

### npm

```
npm i -D typescript
```

iがinstallの略。-Dでdev dependency

### yarn

```
yarn add typescript -D 
```

## ローカルパッケージの実行

### npm

```
npx {package}
```

### yarn

```
yarn -s run {package}
```
　
### たとえばtsc init

```
yarn -s run tsc --init
```
