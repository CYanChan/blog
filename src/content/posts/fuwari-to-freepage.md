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
部署命令：`npx wrangler deploy --assets=./dist`    
![](../assets/images/fuwari-to-freepage-4.png)
如果卡在最后一步无法部署，就在根目录新建一个 `wrangler.toml` 并推送到仓库中    
```js title="wrangler.toml"
name = "blog" # Pages项目名
compatibility_date = "2025-11-12" # 当前日期
```
构建完成后打开页面即可，你也可以添加一个自定义域
![](../assets/images/fuwari-to-freepage-5.png)