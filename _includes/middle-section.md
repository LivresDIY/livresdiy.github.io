## {{ site.data.content.middle.title }}

{{ site.data.content.middle.description }}

<div class="highlight">{{ site.data.content.middle.highlight }}</div>

{{ site.data.content.middle.intro }}

<ul class="features-list">
{% for feature in site.data.content.middle.features %}
  <li><strong>{{ feature.title }}</strong><br>{{ feature.description }}</li>
{% endfor %}
</ul>

<div class="cta-section">
  <a href="{{ site.data.content.middle.cta_link }}" class="btn">{{ site.data.content.middle.cta_text }}</a>
</div>
