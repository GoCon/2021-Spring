---
key: b4-l
title: ホットリロードツールの作り方
id: b4-l
format: conference
talkType: long_session
level: all
tags:
  - B4-L
speakers:
  - makki_d
videoId: null
presentation: null
draft: false
---
サーバプログラムを書いている時、ソースコードを書き換えるたびにビルド・再起動するのは手間です。
このようなとき、ソースコードの変更を検知して、自動でビルド・再起動してくれるホットリロードツールが便利です。
Go言語でも、realizeやairなど、いくつものホットリロードツールが公開されています。

ホットリロードツールに必要な機能は大きく分けて次の2つです。

1. ファイルの更新を監視する
2. プログラムを起動・再起動する

拙作のシンプルな汎用ホットリロードツール「arelo」において、これらの機能をどのように実装しているかを解説します。
