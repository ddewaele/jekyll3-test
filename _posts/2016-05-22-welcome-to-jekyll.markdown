---
layout: post
title:  "Welcome to Jekyll!"
date:   2016-05-22 21:00:03 +0200
categories: jekyll update
---


| Variable         | Value               | Rmark                                                                  |
|:----------------:|:------------------- | ---------------------------------------------------------------------- |
| site.github.url  | {{site.github.url}} | set automatically when deployed on github, empty otherwise             |
| site.baseurl     | {{site.baseurl}}    | set in _config.yml, used to prepend urls                               |
| site.url         | {{site.url}}        | set in _config.yml (used for the canonical link (SEO) and in the feed) |


Logic should be something like this

```
if site.github.url!=null  site.github.url = site.url + site.baseurl
```


[Clearing Up Confusion Around Baseurl](http://blog.parkermoore.de/2014/04/27/clearing-up-confusion-around-baseurl/)

````
baseurl: "/jekyll3-test" # the subpath of your site, e.g. /blog
```