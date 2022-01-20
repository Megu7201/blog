---
title: Hexo Sagiri 主題設置
date: 2022-01-19 13:38:59
tags: hexo
---

在 Github 看到 DIYgod 大神寫的 [Sagiri 主題](https://github.com/DIYgod/hexo-theme-sagiri) 卻因為 hexo 有更改一些預設模組、還有路徑的設置導致無法直接使用，在此寫一個小小教學提供大家參考。

# Clone 
```bash
cd {your hexo folder}/themes
git clone https://github.com/DIYgod/hexo-theme-sagiri.git {custom_name}
```
# Install modules
```bash
npm i nprogress
npm i balloon-css
```

# Modify Path
```bash
# {your_folder}/themes/{custom_name}/css/main.styl
# change @import "../../node_modules/nprogress/nprogress.css" to
@import "../../../node_modules/nprogress/nprogress.css"

# change @import "../../node_modules/balloon-css/balloon.css" to
@import "../../../node_modules/balloon-css/balloon.css"

```

# Run Server
```bash
hexo server
```