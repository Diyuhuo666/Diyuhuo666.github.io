---
layout: default
title: Home
---

# Welcome to My Site! 👋

Hi there! I'm **Diyuhuo666**.

This is my personal website built with Jekyll and hosted on GitHub Pages. Here you'll find my projects, blog posts, and more.

## About Me

- 🎓 Student & Developer
- 💻 Passionate about coding and technology
- 🚀 Always learning new things

## Latest Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — *{{ post.date | date: "%Y-%m-%d" }}*
{% endfor %}

---

Stay tuned for more updates!
