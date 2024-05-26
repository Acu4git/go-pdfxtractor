# 概要

このアプリは，京都工芸繊維大学が掲載している奨学金一覧から，自分が対象に含まれるような項目を取り出してまとめる目的で作成しています（制作途中）．

# 使い方（予定）

```
go run main.go -t undergraduate
```

`-t`: 対象（undergraduate，graduate）

# 実装予定

- クローラーを用いて動的に pdf ファイルへの URL を取得する
- flag を用いた引数の実装
- いちいちローカルにファイルを作成せずに，レスポンスから直接操作できるようにする
