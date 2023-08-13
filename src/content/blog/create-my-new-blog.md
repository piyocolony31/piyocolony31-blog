---
author: Eunsol
pubDatetime: 2023-08-12T11:23:00+09:00
title: Astroで新しいブログを作成しました
postSlug: create-my-new-blog
featured: false
draft: false
tags:
  - astro
  - blog
ogImage: ""
description:
  人生で初めてブログを自作しました。想定していたよりも大変でした。
---

## 自分のブログを作りたかった理由

- ポートフォリオとして活用するため
- 自分自身を知ってもらう場を作りたかったため
- 技術ブログとして情報を発信するため

## なぜAstroを選んだか

- AstroはThemeが豊富であり、私の好みのものがあったため
- Next.jsを使用するほどブログに高機能な要件は不要だったため

## Astroを使ってみた感想

- Astroには様々なThemeがあり、お洒落なデザインなものが多く、どのThemeを選ぶのか考えるのが楽しかったです。
- ブログの雛形を作成するところまでは、AstoroのThemeを使用することで簡単にブログを作成することができましたが、そこから調整を加える段階では、知らない知識を都度調べる必要があり、想定していたよりも大変でした。

## 頑張ったところ

- 「Social Links」機能について、Theme側ではデフォルトで提供されていなかったZennのアイコンとリンクを追加し、自身のZennページへ遷移する導線を作成しました。

## 大変だったところ

- ブログ記事の投稿時間がUSTになってしまう問題が発生しました。これはローカル開発環境では再現せず、Vercel環境にデプロイした後に発生しました。問題の切り分けが難しく、Vercelのタイムゾーンを制御する方法を調べたり、AstroのReactコンポーネントにconsole.logを差し込み、該当の値をデバッグし、問題を解消しました。
- Themeが生成したTailWindCSSで作られたマークアップに修正を加えるのが難しかったです。

## 今後ブログに追加してみたい機能

- ブログのタイトルを「EunsolBlog」から「Eunsol Blog」に変更する
- 「Social Links」のアイコン押下時にリンク先が新しいタブで開くようにする
- コメント機能を追加する

## 参考情報

Astro でブログを作成する！<br>
<https://zenn.dev/eunsol_seo/scraps/0b87357602a3d2>

Vercel環境でタイムゾーンがズレる場合の対処法<br>
<https://blog.junpeko.com/consider-vercel-timezone>

JavaScript: date-fnsでタイムゾーンを扱う<br>
<https://qiita.com/suin/items/296740d22624b530f93a>
