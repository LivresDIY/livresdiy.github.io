---
layout: none
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>{{ site.title }}</title>
  <meta name="description" content="{{ site.description }}">
  <link rel="stylesheet" href="{{ "/assets/main.css" | relative_url }}">
</head>
<body>
  <main class="page-content" aria-label="Content">
    <div class="wrapper">
      
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
      
    </div>
  </main>
</body>
</html>
