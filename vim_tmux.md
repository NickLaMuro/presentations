---
layout: deck-js
title: "Vim + Tmux: How to make Vim your IDE for cross language development"

---

{% for slide in site.categories.vim-tmux %}
  <section class="slide" id="{{ slide.categories.first }}">
    {{ slide.content }}
  </section>
{% endfor %}
