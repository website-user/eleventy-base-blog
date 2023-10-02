---
layout: layouts/base.njk
eleventyNavigation:
  key: Games
  parent: Other Stuff
  order: 2
---
# Games

I like playing games - but more than playing them I like _making_ games. Here are a few I've made.

<div class="portfolioLayout">   
    {% for post in collections.game %}
      <div class="portfolioItem">
        <a href="{{post.url}}">
          <img class="portfolioImage" src="{{post.data.cover}}">
        </a>
        <h3> 
          <a href="{{post.url}}">{{post.data.title}}</a>
        </h3>
      </div>
    {% endfor %}
</div>
