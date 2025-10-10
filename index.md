---
layout: post
---
<h1>{{ site.title }}</h1>
<hr>
<h3>2025MAG data</h3>

{%- assign magPages = site.2025.pages | where: "discipline", "MAG" -%}
    {%- for page in magPages -%}
        <p><a href="{{ post.url }}">{{ post.title }}</a></p>
    {%- endfor -%}

<h2>WAG posts</h2>

{%- assign wagPosts = site.posts | where: "discipline", "WAG" -%}
    {%- for post in wagPosts -%}
        <p><a href="{{ post.url }}">{{ post.title }}</a></p>
    {%- endfor -%}

<!-- <h2>Artistic posts</h2>

{%- if discipline == "MAG" or discipline == "WAG" -%}
{%- assign artisticPosts = true -%}
{%- endif -%}

  {%- for post in artisticPosts -%}
     <p><a href="{{ post.url }}">{{ post.title }}</a></p>
  {%- endfor -%} -->

<!--  {%- assign artisticPosts = site.posts | where: "rating", "FIG 2" -%}
  {%- assign artisticPosts = site.posts | where: "rating", "FIG 3" -%}
{%- for post in artisticPosts -%}
        <p><a href="{{ post.url }}">{{ post.title }}</a></p>
    {%- endfor -%} -->

<h2>Pages</h2>
    {%- for page in site.pages -%}
        {%- if page.title -%}
            <p><a href="{{ page.url }}">{{ page.title }}</a>!</p>
        {%- endif -%}
    {%- endfor -%}
