---
layout: layouts/base.njk
eleventyNavigation:
  key: Portfolio
  order: 2
---
# Portfolio

I am a person that writes stuff.
More changes  
Changes changes changes

<section class="portfolio-section">
    {% for item in collections.portfolio %}
        <article class="portfolio-item">
            <h2>{{ item.data.title }}</h2>

            {% if item.data.imagePath %}
                <img src="{{ item.data.imagePath }}" alt="{{ item.data.title }} Image">
            {% endif %}

            <p>{{ item.data.description }}</p>

            <a href="{{ item.url }}">Read more</a>
        </article>
    {% endfor %}
</section>