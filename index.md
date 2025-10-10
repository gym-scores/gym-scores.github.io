---
layout: post
---
<h1>{{ site.title }}</h1>
<hr>
<h2>Recent meets</h2>
    {%- for post in site.posts -%}
        <p><strong>Post title:</strong> <a href="{{ post.url }}">{{ post.title }}</a></p>
    {%- endfor -%}

<h2>MAG posts</h2>

{%- assign magPosts = site.posts | where: "discipline", "MAG" -%}
    {%- for post in magPosts -%}
        <p><a href="{{ post.url }}">{{ post.title }}</a></p>
    {%- endfor -%}

<h2>WAG posts</h2>

{%- assign wagPosts = site.posts | where: "discipline", "WAG" -%}
    {%- for post in wagPosts -%}
        <p><a href="{{ post.url }}">{{ post.title }}</a></p>
    {%- endfor -%}

<h2>Artistic posts</h2>

{% if discipline == "MAG" or discipline == "WAG" %}
  {% assign artisticPosts = site.posts %}
{% endif %}
{% for post in artisticPosts -%}
        <p><a href="{{ post.url }}">{{ post.title }}</a></p>
    {%- endfor -%}
    
<h2>Pages</h2>
    {%- for page in site.pages -%}
        {%- if page.title -%}
            <p><a href="{{ page.url }}">{{ page.title }}</a>!</p>
        {%- endif -%}
    {%- endfor -%}
