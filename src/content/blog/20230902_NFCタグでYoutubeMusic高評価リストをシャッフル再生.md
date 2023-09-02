---
author: piyocolony31
pubDatetime: 2023-09-02T13:00:00+09:00
title: 【Android】NFC ToolsのみでYoutubeMusic高評価リストをシャッフル再生する方法
postSlug: 20230902-nfc-youtube-music
featured: false
draft: false
tags:
  - nfc
  - hobby
ogImage: ""
description: 課金不要
showToc: true
---

## NFC タグでお気に入りの曲をシャッフル再生したい！

NFC タグ､マイブーム来てます｡

[ctunk(NFC タグ専門店) 累計 10 万枚突破 シールタイプ (NTAG216/888 バイト) iPhone 対応 android 対応 セサミ対応 (10 枚入)](https://www.amazon.co.jp/dp/B0CB1VPDQR)

NFC タグが余っていたので､NFC タグにワンタッチでお気に入りの音楽を流せるようにしてみました｡

この記事では、NFC タグにタッチしたら YouTube Music の高評価リストをシャッフル再生させる方法について解説します。

## 環境・ツール

- Android スマートフォン
- NFC タグ
- NFC Tools アプリ [GooglePlay リンク](https://play.google.com/store/apps/details?id=com.wakdev.wdnfc&hl=ja&gl=US)

## やり方

### NFC Tools アプリで「タスク」タブを開いて「タスクを追加」

<img src="/assets/post/20230902-nfc-youtube-music-before.jpeg" width="30%">

NFC Tools アプリで「タスク」タブを開き､「タスクを追加」をタップします｡

### 「アプリ」→「URL/URI」をタップし､URL を入力し OK

「アプリ」→「URL/URI」の順にタップして､URL 入力画面では以下の URL を入力してください｡

https://music.youtube.com/watch?list=LM&shuffle=1

OK を押すと下の画像の状態になり書き込む準備ができます｡

<img src="/assets/post/20230902-nfc-youtube-music-after.jpeg" width="30%">

### 書き込む

最後に上のスクショの「書く / 93 バイト」をタップして NFC タグにスマホを近づけて書き込んで完了です｡

## つまづきポイント解説

### NFC Tools の「書く」タブと「アプリ」タブの違い

<img src="/assets/post/20230902-nfc-youtube-music-tab.png" width="30%">

「書く」タブでも URL 書き込みはできますが､YoutubeMusic アプリではなくブラウザが開いてしまいます｡

アプリを開きたい場合は「タスク」タブから URL を書き込みましょう｡

|            | 「書く」タブ | 「タスク」タブ |
| ---------- | ------------ | -------------- |
| 開くアプリ | ブラウザ     | Youtube Music  |

### Youtube Music で高評価プレイリストを自動再生をする方法

NFC タグでアプリに期待する動作をさせたい場合､アプリごとに決められた intent で指定することができます｡
一方でこの方法はアプリごとに挙動が違うのでトライアンドエラーが必要になります｡

Youtube Music もこの intent を使った方法を覚悟してましたが､以下の reddit で同じ悩みを持つ人が URL を使った簡単な方法を紹介していました｡

[reddit: Playing liked songs on YouTube Music : r/tasker](https://www.reddit.com/r/tasker/comments/ojghn1/playing_liked_songs_on_youtube_music/)

## 余談

この記事の内容にたどり着くまで色々試行錯誤した中で得た有益情報を共有です｡

NFC Tools では Tasker というタスク実行アプリと連携することができます｡

Tasker は有料アプリですが､公式 HP からトライアル版 apk をダウンロードできます｡

軽く試したいときはおすすめです｡

[Tasker for Android 公式 HP](https://tasker.joaoapps.com/download.html)
