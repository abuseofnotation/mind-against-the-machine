---
layout: default
---

<div class="chapter-zero">

    <div class="book-title">
      <a href="{{site.baseurl}}/dont-fear/">
      <h1>Don't fear</h1>
      </a>
    </div>
        <div class="artwork">
        <img class="comic-web-panel" src="./comic/04.svg" alt="
{{page.image}}
        "></img>
        </div>

        <h2>{{page.subtitle}}</h2>

        <div class="prev-next">
        {% if page.previous.url %}
          <a class="button" href="{{site.baseurl}}{{page.previous.url}}">&laquo;prev</a>
        {% endif %}
        {% if page.next.url %}
          <a class="button" href="{{site.baseurl}}{{page.next.url}}">next&raquo;</a>
        {% endif %}
        </div>

        <div class="scope"></div>
{{ content }}

        <div class="prev-next">
        {% if page.previous.url %}
          <a class="button" href="{{site.baseurl}}{{page.previous.url}}">&laquo;prev</a>
        {% endif %}
        {% if page.next.url %}
          <a class="button" href="{{site.baseurl}}{{page.next.url}}">next&raquo;</a>
        {% endif %}
        </div>
  <!--

  {% for post in site.confusion-breeds-clarity%}
  <article class="chapter-preview {% if post.url == page.url %} chapter-underline {% endif %}">
        <p>

        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
        <i>{{ post.subtitle }}</i>
        </p>

    </article>
  {% endfor %}
  -->
</div>
