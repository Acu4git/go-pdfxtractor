# 概要

このアプリは，京都工芸繊維大学が掲載している奨学金一覧から，自分が対象に含まれるような項目を取り出してまとめる目的で作成しています．

# 開発環境

- go1.22.4 linux/amd64
- Python 3.10.12
- Ubuntu 22.04.4 LTS on Windows 10 x86_64

# 使い方

extractor では requirements.txt から pip install をお願いします．

```bash
pip install -r requirements.txt
```

また，Go の各モジュール(scraper, tabular)にて go mod tidy しておいてください

```bash
go mod tidy
```

プロジェクトのルートディレクトリにて実行

```bash
source run.sh
```

<!-- `-t`: 対象（undergraduate，graduate）(追加予定) -->

2024 年 6 月 28 日
現時点では，奨学金情報を一括で出力するようにしています

# 実装予定

- 引数を指定し，必要な情報だけ抽出できるようにする
- いちいちローカルにファイルを作成せずに，レスポンスから直接操作できるようにする
- python または Go 言語 のみで実装
- Web で公開することで，環境構築をしなくても使えるようにする
