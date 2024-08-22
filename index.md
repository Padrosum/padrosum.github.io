---
title: "Ana Sayfa"
layout: default
---

# Hoş Geldiniz

Ben Padros, uzun zamandır **X**'ten felsefî ve teolojik paylaşımlar yapıyorum. Bulunduğum pozisyonun radikâl olduğunu elbette biliyor ve  
geleneğin getirdiği her argümana karşı iki argüman getirmeye özen gösteriyorum.

## Blog Yazıları

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
*Yayınlanma Tarihi:* {{ post.date | date: "%d %B %Y" }}

{{ post.excerpt }}

---

{% endfor %}
