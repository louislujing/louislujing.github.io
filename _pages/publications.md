---
layout: page
title: Publications
permalink: /publications/
years: [2020,2019,2018,2017,2016,2015,2014]
---

# Publications

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography --template bib -q @*[year={{y}}]* %}
{% endfor %}

Other publication lists:

[APA style][1] \| [BibBase][2] \| [Google Scholar][3] \| [ResearchGate][4]

[1]: {{ site.baseurl }}/publications-normal/
[2]: {{ site.baseurl }}/publications-bibbase/
[3]: https://scholar.google.com/citations?user=WMLzC7IAAAAJ&hl
[4]: https://www.researchgate.net/profile/Lu_Jing4/research