---
layout: page
permalink: /publications/
title: 论文成果
description: 实验室发表的学术论文与研究成果。
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

本页收录王斑老师参与发表的期刊论文与会议论文（含会议论文集章节），不限定作者排序。两类成果分别展示，并按发表年份由近及远排列。点击论文条目中的链接可访问出版页面。

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

## 会议论文

{% bibliography --query @inproceedings %}

</div>
