---
layout: post
title: "Hello Octopress"
date: 2012-12-14 01:14
comments: true
categories: Misc
---

日記用の軽いブログなどは幾つか持っているのですが、前々から技術系のブログをひとつ作りたかったので Octopress + GitHub Pages で構築してみました。人に見られることを想定したブログというものはここ数年作っていなかったので本当に久しぶり。主に技術ネタを扱っていきたいと思っているので横幅を広く取れるテーマにしてみました。以下備忘録。

## ブログの設定を変更したとき

```
$ git add .
$ git commit -m 'message'
$ git push origin source
```

## 記事を書くとき

```
$ bundle exec rake new_post["title_in_english"]
$ vim source/_posts/your_new_post.markdown
$ bundle exec rake generate
$ bundle exec rake preview -- http://localhost:4000
$ bundle exec rake gen_deploy
```