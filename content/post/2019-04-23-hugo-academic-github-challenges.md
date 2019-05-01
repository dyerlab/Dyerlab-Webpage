---
title: Hugo + Academic _ Github Challenges
author: rodney
date: '2019-04-23'
slug: hugo-academic-github-challenges
categories:
  - R
tags:
  - blogdown
  - hugo
cover: "/img/hello.jpg"
---

So one of the things I found to be necessary is that when you clone the git repository for academic-kickstarter, you need to give the following command in your root directory.

```
git submodule update --init --recursive
```

Or it will give you a bunch of odd erros saying crazy stuff like:

```
found no layout file for "HTML" for "page"
```
