---
title: Games
layout: layouts/base.njk
eleventyNavigation:
  key: Games
  parent: Other Stuff
  order: 2
---



<style>
.portfolioLayout {
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(20em, 1fr));
	grid-gap: 2em;
}

.portfolioImage {
	width: 100%;
	height: 226px;
  object-fit: cover;
  border-radius: 2px;

}

.portfolioItem {
    /* This makes sure the image and title inside it stack vertically */
    display: flex;
    flex-direction: column;
    align-items: center; /* Optional: to center items horizontally */
    border-style: solid;
    border-width: thick;
    border-color: red;
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

<h1>Games</h1>

Here are some games.

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
