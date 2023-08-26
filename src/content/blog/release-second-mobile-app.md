---
author: piyocolony31
pubDatetime: 2023-08-13T13:57:00+09:00
title: Flutterでポモドーロタイマーアプリを開発してリリースしました
postSlug: release-second-mobile-app
featured: false
draft: false
tags:
  - portfolio
  - flutter
ogImage: ""
description: 20日かけて2つ目のモバイルアプリを開発してリリースしました。
---

## ポモドーロタイマーアプリを作った理由

- [Nomad Coders](https://nomadcoders.co/flutter-for-beginners)という様々なプログラミング言語やフレームワークを学ぶことができるサービスの Flutter の講義でポモドーロアプリを作成するコースがあり、参考にできると思ったため
- 講義の内容に加えて、自分で調べながら追加機能を開発することでスキルの向上につながると思ったため
- ポートフォリオとして活用するため

## ポモドーロ・テクニックとは

> 1980 年代にイタリア人のフランチェスコ・シリロ（フランチェスコ・チリッロ、伊: Francesco Cirillo）によって考案された時間管理術。このテクニックではタイマーを使用し、一般的には 25 分の作業と短い休息で作業時間と休息時間を分割する。1 セットを「ポモドーロ」と呼ぶ。これはイタリア語で「トマト」を意味する言葉で、シリロが大学生時代にトマト型のキッチンタイマーを使用していたことにちなむ。
> ポモドーロ・テクニックを元に、ポモドーロ・タイマー[1]と呼ばれるタイマーが存在し、勉強や作業タスクの効率化の面においてのメリットが注目され近年話題となっている。<br>
> 参照：[ポモドーロ・テクニック - Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%9D%E3%83%A2%E3%83%89%E3%83%BC%E3%83%AD%E3%83%BB%E3%83%86%E3%82%AF%E3%83%8B%E3%83%83%E3%82%AF)

## ポモドーロタイマーアプリの機能

- タイマー機能
- タイマーの一時停止機能
- タイマーのリセット機能
- ポモドーロ回数のカウント機能
- タイマーの時間の変更機能

## ポモドーロタイマーアプリをリリースしてみた感想

- Nomad Corders の講義ではタイマーをリセット機能と変更機能が無かったので、自分で調べながら機能を実装する必要がありました。その流れでタイマーを変更するのに必要な時間を選択する Widget のパッケージをインストールしてアプリへ反映する方法を知りました。
- その後、Google Play へのリリースはスムーズに行うことができましたが、App Store の審査は通りませんでした。App Store Review という審査の問い合わせ窓口に審査に落ちた理由を聞いたところ、[Guideline 4.3 - Design](https://developer.apple.com/app-store/review/guidelines/#spam) を満たしていないためという回答をもらいました。すなわち、類似なアプリが多いため、もう少し特徴的な機能、UI を加える必要があるようです。自分で開発したモバイルアプリが初めて審査に落ちたためショックでした。

## 今後改修したい点

App Store へのリリースに向けて以下の点を改修したいと思います。

- 機能の追加
  - タイマーが終わり次第、5 分間の休憩に自動的に入る機能
  - ポモドーロ回数のリセット機能
- UI の改善
  - キャラクターのイラストを追加し、もっとユニークな UI に変更する

## 参考情報

Pomodoro - Simple Version<br>
Android 版：<https://play.google.com/store/apps/details?id=pomodoro.simple.version>

タイマーを変更する Widget のパッケージ<br>
<https://pub.dev/packages/flutter_material_pickers>

【Flutter 学習ログ】Nomad Coders の Code Challenge を通して Flutter/Dart の知識を深める！ - Zenn<br>
<https://zenn.dev/piyocolony31_seo/scraps/3e0b33da68d40b>
