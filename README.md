## Elena Bonmatí personal site 

My site is hosted in GitHub, using GitHub Pages and Jekyll's theme Voyager. 

## Voyager

Jekyll theme Demo: <http://redvi.github.io/voyager>

### Features:

All HTML files are compressed (see `_layouts/compress.html`).


**Page**

If page contains `active` tag, it will be show on site menu.

```
---
layout: page
title: "About"
permalink: /about/
active: about
---
```

**Post**

All post settings can be changed. Example:

```
---
layout: post
bg: '2016/background.jpg'
title: "Post Heading"
crawlertitle: "page title"
summary: "post description"
date: 2016-06-29
tags : ['front-end']
slug: post-url
author: "Author"
categories: posts
---
```

`bg` is a path to background of your article. By default backgrounds are placed in the `assets/images` directory.

**Relative paths**

If your blog is not in the root directory, you can include images with a relative path. For example:

```
![my_image]({{ site.images | relative_url }}/image.jpg)
```

## Production environment

Build for production:

`JEKYLL_ENV=production jekyll build`
