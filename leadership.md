---
layout: page
title: Leadership
comments: false
permalink: /leadership/
---


<div id="leadership">
{% for author in site.data.authors %}
<h4>{{ author[1].position }} - {{ author[1].name}}</h4>
<!-- <amp-img src="{{ site.baseurl }}{{ author[1].assets }}" alt="{{author[1].name}}" height="30" width="30"></amp-img> -->
<p class="bio">{{ author[1].bio }}</p>
<ul class="ampstart-social-follow list-reset flex items-center flex-wrap m0 mb4">
{% if author[1].github %}
<li>
        <a href="https://github.com/{{author[1].github}}" target="_blank" class="inline-block p1" aria-label="Link to AMP HTML github"><svg xmlns="http://www.w3.org/2000/svg" width="19" height="19" viewBox="0 0 64 64"><path d="M22.4 1.4C-.8 9-7.4 38.4 10.5 54.9 14.7 58.8 20.4 62 23 62c.5 0 1-1.6 1-3.5 0-3.3-.2-3.5-3.5-3.5-3.5 0-4.2-.5-9-6.6-4.4-5.6-2.3-6.2 3.2-.9 4.2 4 7.5 4.5 9.8 1.2 1.4-2.1 1.4-2.2-.7-3-6-2.3-8.8-4.2-10.2-7.2-2.1-4.3-2.1-12.4 0-15.3.8-1.2 1.2-2.7.9-3.2-1-1.6.5-7 1.8-7 .7 0 2.4.6 3.8 1.4 1.7.9 6 1.4 11.9 1.4s10.2-.5 11.9-1.4c1.4-.8 3.1-1.4 3.8-1.4 1.3 0 2.8 5.4 1.8 7-.3.5.1 2 .9 3.2 1.8 2.5 2.1 10.3.7 14.1-1.4 3.6-5 6.6-9.3 7.8-3.3.9-3.7 1.2-2.8 2.9.5 1 1 4.6 1 7.9 0 3.5.4 6.1 1 6.1 5.2 0 15.8-8.8 19.8-16.5 2.3-4.3 2.7-6.3 2.7-13.5 0-7-.4-9.4-2.4-13.5C57.9 12.2 51.8 6 45.6 3 39.6.2 28.5-.6 22.4 1.4z" class="ampstart-icon ampstart-icon-github"/></svg></a>
</li>
{% endif %}
</ul>
<hr>
{% endfor %}
</div>
