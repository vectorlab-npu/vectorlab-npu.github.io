---
layout: lab-en
permalink: /en/publications/
translation: /publications/
title: Publications
description: Journal articles and research results from VECTOR Lab.
lab_nav_order: 1
---

Selected journal articles are listed below. See [Google Scholar](https://scholar.google.com/citations?user=pRjl44sAAAAJ&hl=en) for the full publication list.

<style>
  .publications .author em {
    font-weight: 700;
  }
</style>

{% include bib_search.liquid %}

<div class="publications" markdown="1">

## Journal Articles

{% capture journal_articles %}{% bibliography --query @article %}{% endcapture %}
{{ journal_articles | replace: '第一作者', 'First author' | replace: '通讯作者', 'Corresponding author' | replace: '共同作者', 'Co-author' }}

</div>
