# Welcome to pi-docs
Thanks for dropping by. These pages are dedicated to systematically approaching the pi as a personal computer. I'm cataloging important steps to help myself later and maybe even help some others.

## Table of Contents
{% for item in site.data.navigation.toc %}
    ### {{ item.title }}
        {% for entry in item.subfolderitems %}
          -({{ entry.url }})[{{ entry.page }}]
        {% endfor %}
  {% endfor %}
