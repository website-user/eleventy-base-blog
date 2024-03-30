---
title: Challenge
layout: layouts/base.njk
eleventyNavigation:
  key: Challenge
  parent: Other Stuff
  order: 1
---
<style>
  .box {
  border: 2px solid var(--text-color);
  padding: 1em;
  border-radius: 3px;
  width: 60%;
  }

  @media (max-width: 700px) {
  .box {
    width: 100%; /* Set width to 100% for mobile */
  }
  } 

  input[type=submit] {
  cursor: grabbing;
  background-color: var(--background-color); 
  color: var(--text-color);
  border: 2px var(--text-color);
  border-radius: 3px;
  border-style: solid;
  padding: 14px 16px;
  transition: 0.08s;
  font-size: 17px;  
}

input[type=submit]:hover {
  background-color: var(--text-color);
  color: var(--background-color); 
}

#challenge_content {
  /* Set height */
  height: 60px; /* Adjust the value as needed */

  /* Set width */
  width: 100%; /* Adjust the value as needed */
}

</style>

# Challenges

Here you can challenge me to any kind of game or competition, or challenge a position I hold.  

I'm especially excited to be challenged to play a game you've invented.  

There is no guarantee the challenge will be accepted.  

Good luck.

<br>

<div class="box">

  ## Submit a Challenge

  <form action="https://formspree.io/f/xoqgkdzd" method="post">
    <div>
      <label for="fname">Your Name</label><br>
      <input type="text" id="fname" name="fname" value="" required><br>
    </div>
    <br>
    <div>
      <label for="_replyto">Your Email</label><br>  
      <input type="email" name="_replyto" required>
    </div>
    <br>
    <div>
      <label for="challenge_content">Your Challenge</label><br>  
      <textarea id="challenge_content" name="challenge" rows="4" cols="46" placeholder="Please be specific. Include a time, place, and rules." required></textarea>
    </div>
    <br>
    <!-- <input type="image" name="submit" src="/img/liam_drawing.svg" alt="Submit" style="width: 100px"/> -->
    <input type="submit" value="Challenge Liam"> 
    

  </form> 
</div>

<br>

## Past Challenges
    {% for post in collections.challenge %}
      <h4> 
        <a href="{{post.url}}">{{post.data.title}}</a>
      </h4>
    {% endfor %}