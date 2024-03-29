---
title: Art
layout: layouts/base.njk
eleventyNavigation:
  key: Art
  parent: Other Stuff
  order: 6
---
<style>

body {
  max-width: 76em;
}

.portfolioLayout {
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(17em, 1fr));
	grid-gap: 2em;
}

.portfolioImage {
	width: 18em;
	height: 12em;
  object-fit: cover;
  border-radius: 2px;
}


.organizationImage {
	width: 14em;
	height: 12em;
  object-fit: cover;
  border-radius: 2px;
}

.portfolioItem {
    /* This makes sure the image and title inside it stack vertically */
    display: flex;
    flex-direction: column;
    align-items: center; /* Optional: to center items horizontally */
}

.portfolioItem h3 {
	/* this reduces the spacing between the text and image. */
    margin-top: 0; 
}

.portfolioItem a {
	/*This removes the underline from post title*/
	text-decoration: none;
}
</style>


# Art

<br>
<br>
<br>


<div class="portfolioLayout">   
    {% for post in collections.art %}
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
