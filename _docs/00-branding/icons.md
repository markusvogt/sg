---
title: Icons
info: Icons used in this product.
maturity: alpha
---

<section class="sg-branding">
  <ul class="icon-set">
    {% for image in site.static_files %}
      {% if image.path contains 'src/assets/icons' %}
      <li>
        <img src="{{ site.baseurl }}{{ image.path }}" alt="image" />
        <p><code>{{ image.path }}</code></p>
      </li>
      {% endif %}
    {% endfor %}
  </ul>
</section>
