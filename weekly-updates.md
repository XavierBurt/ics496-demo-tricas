---
layout: page          
title: "Weekly Updates"
permalink: /weekly-updates/
---

<ul class="weekly-list">
  {%- for wk in site.weekly reversed -%}
    <li>
      <a href="{{ wk.url | relative_url }}">
        {{ wk.date | date: "%b %-d, %Y" }} – {{ wk.title | escape }}
      </a>
    </li>
  {%- endfor -%}
</ul>
