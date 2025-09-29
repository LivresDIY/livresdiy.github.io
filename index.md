---
layout: clean
---

<section class="hero-section">
{% capture hero_content %}{% include hero-section.md %}{% endcapture %}
{{ hero_content | markdownify }}
</section>

<section class="middle-section">
{% capture middle_content %}{% include middle-section.md %}{% endcapture %}
{{ middle_content | markdownify }}
</section>

<section class="bottom-section">
{% capture bottom_content %}{% include bottom-section.md %}{% endcapture %}
{{ bottom_content | markdownify }}
</section>
