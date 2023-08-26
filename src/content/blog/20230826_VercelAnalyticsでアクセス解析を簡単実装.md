---
author: piyocolony31
pubDatetime: 2023-08-26T19:35:00+09:00
title: VercelAnalyticsでアクセス解析を簡単実装
postSlug: 20230826-vercel-analytics
featured: false
draft: false
tags:
  - blog
  - astro
  - vercel
ogImage: ""
description: 5分でアクセス解析
---

## 静的サイトでアクセス解析がしたい

## やりかた

[公式の QuickStart](https://vercel.com/docs/analytics/quickstart)のとおりです。

今回は Astro での導入方法を記載します。
Next.js や Svelte などでの導入方法は[QuickStart](https://vercel.com/docs/analytics/quickstart)を確認してください。

### 1. Vercel Analytics を有効化する

以下の URL からログインして Vercel Analytics を有効化
https://vercel.com/d?to=%2F%5Bteam%5D%2F%5Bproject%5D%2Fanalytics&title=Open+Web+Analytics

### 2. script を呼び出す

index.astro の head タグに以下 script を追記

```
<script>
  window.va = window.va || function () { (window.vaq = window.vaq || []).push(arguments); };
</script>
<script defer src="/_vercel/insights/script.js"></script>
```

### 3. デプロイする

デプロイしてサイトにアクセスしてから Vercel Analytics のページを開くとリアルタイムの解析結果が表示されます。

![Vercel Analytics](/public/post/20230826-vercel-analytics.png)
