---
layout: page
title: 뉴스레터
#background_style: bg-info
background_image: url('/assets/img/backgrounds/image-from-rawpixel-id-1199650-jpeg.jpg')
# Add a link to the the top menu
menus:
  header:
    title: 뉴스레터
    weight: 2

sections:
#- type: paragraph.html
#  section_id: help
#  title: 뉴스레터
#  text: >+
#    우리의 뉴스레터를 모아 놓은 곳입니다.
#
#    * [Markdown Syntax Here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).
#
#    * [John Gruber's original spec](http://daringfireball.net/projects/markdown/).
#
#    * [Github-flavored Markdown info page](http://github.github.com/github-flavored-markdown/).
#
- type: paragraph.html
  section_id: more-to-come
  title: 
#  background_style: bg-info
#  text_style: text-left text-white
#  actions:
#   - title: Markdown is fun!
#     class: btn-info
#     url: '#'
  text: >+
    ### 뉴스레터 모음입니다.
---
<div class="toc" style="text-align:center">
  <ul class="texts">
  {% for item in site.categories.news %}

    <li class="text-title">
      <h3><a href="{{ site.baseurl }}{{ item.url }}">
        {{ item.title }}
      </a></h3> - <em>{{ item.date | date: "%Y년 %-m월 %-d일" }}</em>
    </li>
  {% endfor %}
  </ul>
</div>