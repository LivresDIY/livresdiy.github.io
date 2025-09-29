---
layout: landing
---

<section class="hero-section">
  <div class="container">
    {% capture hero_content %}{% include hero-section.md %}{% endcapture %}
    {{ hero_content | markdownify }}
  </div>
</section>

<section class="content-section" id="about">
  <div class="container">
    {% capture middle_content %}{% include middle-section.md %}{% endcapture %}
    {{ middle_content | markdownify }}
  </div>
</section>

<section class="content-section" id="join">
  <div class="container">
    {% capture bottom_content %}{% include bottom-section.md %}{% endcapture %}
    {{ bottom_content | markdownify }}
  </div>
</section>
