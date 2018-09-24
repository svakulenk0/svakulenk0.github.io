---
layout: page
title: ""
tagline: ""
---
{% include JB/setup %}

<div style="display:block;text-align:left"><a href="./img/sv.jpg" imageanchor="1"><img src="https://sites.google.com/site/svitlanv/home/svitlana-vakulenko.jpg" border="0"></a></div>

<strong>PhD</strong> student in <strong>TU Wien</strong><br>
supervised by <a href="http://polleres.net" target="_blank">Axel Polleres</a> and <a href="https://staff.fnwi.uva.nl/m.derijke/" target="_blank">Maarten de Rijke</a><br>
<br>
Researcher in Institute for Information Business<br>
Vienna University of Economics and Business<br>
<span>1020 Vienna<br>


<font face="Candara"><b>Email:</b> </font><span>svitlana dot vakulenko<span> at </span>wu dot ac<span> dot </span>at<br>


<br>
<a href="./pdfs/CV_Vakulenko.pdf" target="_blank">CV</a> <a href="https://github.com/svakulenk0" target="_blank">GitHub</a> <a href="https://twitter.com/svakulenk0" target="_blank">Twitter</a>
<br>


<br>
My primary research interest relate to Natural Language Understanding and applications, especially Information Retrieval including <b>Conversational Search</b> in semi-structured data sources: Open Data, <b>Knowledge Graphs</b> and Social Media streams.



## News

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
