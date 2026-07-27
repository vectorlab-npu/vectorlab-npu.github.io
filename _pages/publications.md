---
layout: page
permalink: /publications/
title: 论文成果
description: 实验室发表的学术论文与研究成果。
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

代表性期刊论文如下。如需获取完整论文列表，请访问 [Google Scholar](https://scholar.google.com/citations?user=pRjl44sAAAAJ&hl=en)。

<style>
  .publications .author em {
    font-weight: 700;
  }
</style>

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

## 期刊论文

{% bibliography --query @article %}



</div>
