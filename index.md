---
title: "Ana Sayfa"
layout: default
---

# Hoş Geldiniz

Ben Padros, uzun zamandır **X**'ten felsefî ve teolojik paylaşımlar yapıyorum. Bulunduğum pozisyonun radikâl olduğunu elbette biliyor ve  
geleneğin getirdiği her argümana karşı iki argüman getirmeye özen gösteriyorum.

## Blog Yazıları

{% assign posts = site.pages | where_exp: "page", "page.path contains '_posts/'" %}

{% for post in posts %}
### [{{ post.title }}]({{ post.url }})
*Dosya Yolu:* {{ post.path }}

{{ post.content | strip_html | truncatewords: 50 }}

---

{% endfor %}
