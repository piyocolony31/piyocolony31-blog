---
author: piyocolony31
pubDatetime: 2023-08-12T11:23:00+09:00
title: Astroで新しいブログを作成しました
postSlug: create-my-new-blog
featured: false
draft: false
tags:
  - astro
  - blog
ogImage: ""
description: 人生で初めてブログを自作しました。想定していたよりも大変でした。
---

## 自分のブログを作りたかった理由

- ポートフォリオとして活用するため
- 自分自身を知ってもらう場を作りたかったため
- 技術ブログとして情報を発信するため

## なぜ Astro を選んだか

- Astro は Theme が豊富であり、私の好みのものがあったため
- Next.js を使用するほどブログに高機能な要件は不要だったため

## Astro を使ってみた感想

- Astro には様々な Theme があり、お洒落なデザインなものが多く、どの Theme を選ぶのか考えるのが楽しかったです。
- ブログの雛形を作成するところまでは、Astoro の Theme を使用することで簡単にブログを作成することができましたが、そこから調整を加える段階では、知らない知識を都度調べる必要があり、想定していたよりも大変でした。

## 頑張ったところ

- 「Social Links」機能について、Theme 側ではデフォルトで提供されていなかった Zenn のアイコンとリンクを追加し、自身の Zenn ページへ遷移する導線を作成しました。

## 大変だったところ

- ブログ記事の投稿時間が UST になってしまう問題が発生しました。これはローカル開発環境では再現せず、Vercel 環境にデプロイした後に発生しました。問題の切り分けが難しく、Vercel のタイムゾーンを制御する方法を調べたり、Astro の React コンポーネントに console.log を差し込み、該当の値をデバッグし、問題を解消しました。
- Theme が生成した TailWindCSS で作られたマークアップに修正を加えるのが難しかったです。

## 今後ブログに追加してみたい機能

- ブログのタイトルを「piyocolony31Blog」から「piyocolony31 Blog」に変更する
- 「Social Links」のアイコン押下時にリンク先が新しいタブで開くようにする
- コメント機能を追加する

## 参考情報

Astro でブログを作成する！<br>
<https://zenn.dev/piyocolony31_seo/scraps/0b87357602a3d2>

Vercel 環境でタイムゾーンがズレる場合の対処法<br>
<https://blog.junpeko.com/consider-vercel-timezone>

JavaScript: date-fns でタイムゾーンを扱う<br>
<https://qiita.com/suin/items/296740d22624b530f93a>
