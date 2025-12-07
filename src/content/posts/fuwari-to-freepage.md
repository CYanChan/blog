---
title: 把fuwari生成的静态页面托管到各个免费page中
published: 2025-11-12
description: 搞几个备用站点，不然哪天就被一锅端啦
tags:
  - VPS
  - Tech
category: VPS
draft: false
image: ../assets/images/fuwari-to-freepage-1.png
---
## Cloudflare
前往Cloudflare的 Workers 和 Pages 页面，创建一个新Pages
![](../assets/images/fuwari-to-freepage.png)![](../assets/images/fuwari-to-freepage-2.png)
![](../assets/images/fuwari-to-freepage-3.png)
构建命令：`pnpm build`
