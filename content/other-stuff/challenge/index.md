---
layout: layouts/base.njk
eleventyNavigation:
  key: Challenge
  parent: Other Stuff
  order: 1
---
# Issue a challenge

Here you can challenge me to any kind of game or competition, or challenge a position I hold.  

I'm especially excited to be challenged to play a game you've invented.  

There is no guarantee the challenge will be accepted.  
Good luck.

(This is carried over from my old website.
I haven't quite figured out how to do input forms quite yet - so for the time being, if you've got a challenge, email me. )

<br>

## Submit a Challenge
Until I get input forms figured out, see [contact](/contact)

<br>

## Past Challenges
    {% for post in collections.challenge %}
      <h4> 
        <a href="{{post.url}}">{{post.data.title}}</a>
      </h4>
    {% endfor %}

