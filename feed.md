<?xml version="1.0" encoding="UTF-8" ?>
<rss version="2.0">

<channel>
  <title>David's Blog</title>
  <link>https://blog.aboutdavid.me</link>
  <description>My awesome blog</description>
  <copyright>© 2020 aboutDavid. All rights reserved.</copyright>
  
  <!-- Start Items -->
  {% for post in site.posts %}
  <item>
    <title>{{ post.title | xml_escape }}</title>
    <description>{{ post.excerpt | xml_escape }}</description>
    <link>{{ post.url | xml_escape }}</link>
  </item>
  {% endfor %}
</channel>

</rss>
