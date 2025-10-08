---
layout: post
---
<h1>{{ site.title }}</h1>
<hr>
<h2>Recent meets</h2>
    {%- for post in site.posts -%}
        <p><strong>Post title:</strong> {{ post.title }}</p>
    {%- endfor -%}

<h2>MAG posts</h2>

{% assign magPages = site.pages | where: "discipline", "MAG" %}
    {%- for page in magPages -%}
        {{ page.title }}
    {%- endfor -%}

<h2>WAG posts</h2>

{% assign wagPosts = site.posts | where: "discipline", "WAG" %}
    {%- for post in wagPosts -%}
        <p>{{ post.title }}!</p>
    {%- endfor -%}
<h2>Pages</h2>
    {% for page in site.pages %}
        {{ page.title }}!
    {% endfor %}
