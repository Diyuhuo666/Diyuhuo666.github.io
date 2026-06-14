---
layout: default
title: 首页
---

<div class="hero">
  <div class="fire-bg"></div>
  <h1>🔥 欢迎来到地狱火的主页 🔥</h1>
  <p class="hero-sub">这里是地狱火的领地，我在这里分享我的技术探索与创意项目</p>
  <div class="hero-links">
    <a href="#posts" class="btn btn-primary">📖 查看博客</a>
    <a href="{{ '/about' | relative_url }}" class="btn btn-outline">👤 关于我</a>
  </div>
</div>

## 📝 最新博客

<div id="posts" class="post-grid">
{% if site.posts.size > 0 %}
{% for post in site.posts %}
  <div class="post-card">
    <div class="post-card-header">
      <span class="post-icon">📄</span>
      <time>{{ post.date | date: "%Y-%m-%d" }}</>
    </div>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 80 }}</p>
  </div>
{% endfor %}
{% else %}
  <div class="post-card">
    <span class="post-icon">✏️</span>
    <h3>还没有博客文章</h3>
    <p>快去 `_posts` 目录写你的第一篇文章吧！</p>
  </div>
{% endif %}
</div>

## 🔗 快速链接

<div class="links-grid">
  <a href="https://github.com/Diyuhuo666" target="_blank" class="link-card">
    <span class="link-icon">🐙</span>
    <span>GitHub 主页</span>
  </a>
  <a href="mailto:2487935515@qq.com" class="link-card">
    <span class="link-icon">📧</span>
    <span>发送邮件</span>
  </a>
</div>

---

<p class="footer-note">🔥 地狱火永恒燃烧 🔥</p>
