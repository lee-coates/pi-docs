---
---
<h1>Welcome to pi-docs</h1>
Thanks for dropping by. These pages are dedicated to systematically approaching the pi as a personal computer. I'm cataloging important steps to help myself later and maybe even help some others.

<h2>Table of Contents</h2>
{% for item in site.data.navigation.toc %}
    <h3>{{ item.title }}</h3>
      <ul>
        {% for entry in item.subfolderitems %}
          <li><a href="{{ entry.url }}">{{ entry.page }}</a></li>
        {% endfor %}
      </ul>
  {% endfor %}
