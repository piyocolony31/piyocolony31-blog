---
author: Eunsol
pubDatetime: 2023-08-13T13:57:00+09:00
title: Flutterでポモドーロタイマーアプリを開発してリリースしました
postSlug: release-second-mobile-app
featured: false
draft: false
tags:
  - portfolio
  - flutter
ogImage: ""
description:
  20日かけて2つ目のモバイルアプリを開発してリリースしました。
---

## ポモドーロタイマーアプリを作った理由

- [Nomad Coders](https://nomadcoders.co/flutter-for-beginners)という様々なプログラミング言語やフレームワークを学ぶことができるサービスのFlutterの講義でポモドーロアプリを作成するコースがあり、参考にできると思ったため
- 講義の内容に加えて、自分で調べながら追加機能を開発することでスキルの向上につながると思ったため
- ポートフォリオとして活用するため

## ポモドーロ・テクニックとは

> 1980年代にイタリア人のフランチェスコ・シリロ（フランチェスコ・チリッロ、伊: Francesco Cirillo）によって考案された時間管理術。このテクニックではタイマーを使用し、一般的には25分の作業と短い休息で作業時間と休息時間を分割する。1セットを「ポモドーロ」と呼ぶ。これはイタリア語で「トマト」を意味する言葉で、シリロが大学生時代にトマト型のキッチンタイマーを使用していたことにちなむ。
ポモドーロ・テクニックを元に、ポモドーロ・タイマー[1]と呼ばれるタイマーが存在し、勉強や作業タスクの効率化の面においてのメリットが注目され近年話題となっている。<br>
> 参照：[ポモドーロ・テクニック - Wikipedia](<https://ja.wikipedia.org/wiki/%E3%83%9D%E3%83%A2%E3%83%89%E3%83%BC%E3%83%AD%E3%83%BB%E3%83%86%E3%82%AF%E3%83%8B%E3%83%83%E3%82%AF>)

## ポモドーロタイマーアプリの機能

- タイマー機能
- タイマーの一時停止機能
- タイマーのリセット機能
- ポモドーロ回数のカウント機能
- タイマーの時間の変更機能

## ポモドーロタイマーアプリをリリースしてみた感想

- Nomad Cordersの講義ではタイマーをリセット機能と変更機能が無かったので、自分で調べながら機能を実装する必要がありました。その流れでタイマーを変更するのに必要な時間を選択するWidgetのパッケージをインストールしてアプリへ反映する方法を知りました。
- その後、Google Playへのリリースはスムーズに行うことができましたが、App Storeの審査は通りませんでした。App Store Reviewという審査の問い合わせ窓口に審査に落ちた理由を聞いたところ、[Guideline 4.3 - Design](https://developer.apple.com/app-store/review/guidelines/#spam) を満たしていないためという回答をもらいました。すなわち、類似なアプリが多いため、もう少し特徴的な機能、UIを加える必要があるようです。自分で開発したモバイルアプリが初めて審査に落ちたためショックでした。

## 今後改修したい点

App Storeへのリリースに向けて以下の点を改修したいと思います。

- 機能の追加
  - タイマーが終わり次第、5分間の休憩に自動的に入る機能
  - ポモドーロ回数のリセット機能
- UIの改善
  - キャラクターのイラストを追加し、もっとユニークなUIに変更する

## 参考情報

Pomodoro - Simple Version<br>
Android版：<https://play.google.com/store/apps/details?id=pomodoro.simple.version>

タイマーを変更するWidgetのパッケージ<br>
<https://pub.dev/packages/flutter_material_pickers>

【Flutter学習ログ】Nomad Coders の Code Challenge を通して Flutter/Dart の知識を深める！ - Zenn<br>
<https://zenn.dev/eunsol_seo/scraps/3e0b33da68d40b>
