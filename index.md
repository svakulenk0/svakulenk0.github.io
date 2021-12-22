---
layout: page
title: ""
tagline: ""
---
{% include JB/setup %}

<div style="display:block;text-align:left"><a href="./assets/sv.jpg" imageanchor="1"><img src="https://sites.google.com/site/svitlanv/home/svitlana-vakulenko.jpg" border="0"></a></div>

<strong>Machine Learning Scientist</strong> in Alexa AI - Web Information<br>
Amazon, Barcelona, Spain<br>

<font face="Candara"><b>Email:</b> </font><span>svvakul<span> at </span>amazon<span> dot </span>com<br>


<br>
<a href="./pdfs/CV_Vakulenko.pdf" target="_blank">CV</a> <a href="https://github.com/svakulenk0" target="_blank">GitHub</a> <a href="https://twitter.com/svakulenk0" target="_blank">Twitter</a> <a href="https://www.linkedin.com/in/svitlanavakulenko" target="_blank">LinkedIn</a>
<br>


<br>
My primary research interests relate to Natural Language Understanding with application to Information Retrieval, and in particular <b>Conversational Search</b>.



## News

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
