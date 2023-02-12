---
title: Adding Images To A Hexo Blog By Typora The SimpleWay
date: 2022-09-29 02:16:47
tags: Misc
cover: topTodos.jpeg
typora-root-url: AddingImgToHexoBlogByTyporaTheSimpleWay
---

Only 2 steps will do the trick.

## step1

Go to your hexo root directory, and add the line below to `_config.yml`.

```
post_asset_folder: true
```

As a result, every time I run hexo new [fooBlog] command I got a empty [fooBlog] directory in my _posts.

> Hint: switch [fooBlog] to your real blog title.

## step2

Add this line to fooBlog's metadata section.

```json
typora-root-url: fooBlog
```

## sample

Say I have a img named topTodos.jpeg in [fooBlog] directory mentioned above, then my image inserting markdown code will be like:`![](topTodos.jpeg)`

Result:

![topTodos](topTodos.jpeg)

## Reference

First paragraph on https://hexo.io/zh-cn/docs/asset-folders.html

Paragraph 'Relative path to certain folder' on https://support.typora.io/Images/
