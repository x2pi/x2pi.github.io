---
layout: post-l
creationdate:  2018-02-05 00:00:00 +0700
title: Number
permalink: /book/new-language/english/01-number
author: PI
date: 2018-02-05 00:00:00 +0700
---
<script src="http://code.responsivevoice.org/responsivevoice.js"></script>
 |English|Vietnamese|
 | --- | --- |
 {% for number in site.data.language.01-number %}| {{ number[0][0] }} <i class="fa fa-volume-up" onclick="responsiveVoice.speak('{{ number[0][0] }}', 'US English Female')"></i>| {{ number[0][1] }} <i class="fa fa-volume-up" onclick="responsiveVoice.speak('{{ number[0][1] }}', 'Vietnamese Male')"></i>|
 {% endfor %}
 
 
