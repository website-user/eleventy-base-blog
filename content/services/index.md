---
title: Services
layout: layouts/base.njk
eleventyNavigation:
  key: Services
  order: 4
---

<style>
.inline img {
	/*2023-09-27 adding this specifically for the Consulting page*/
	float: left;
	margin: 0px;
	margin-right:20px;
  width:300px;
  height:100%;
}

/* Style the tab */
.tab {
  overflow: hidden;
  border: 1px solid var(--text-color);
  background-color: var(--background-color);
  border-radius: 3px 3px 0px 0px;

}

/* Style the buttons inside the tab */
.tab button {
  background-color: var(--background-color);
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.08s;
  font-size: 17px;
  color: var(--text-color);

}

.tab button:hover {
  color: var(--text-color-link-active);
  text-decoration: underline;
  background-color: var(--background-color);
}

/* Create an active/current tablink class */
.tab button.active {
  text-decoration: underline;
  background-color: var(--text-color);
  color: var(--background-color);
  

}

/* Style the tab content */
.tabcontent {
  display: none;
  padding: 6px 12px;
  border: 1px solid var(--text-color);
  border-top: none; /*this keeps the lines doubling up*/
  min-height: 200px;
  border-radius: 0px 0px 3px 3px; /*cycles through corners starting with top left*/
}
</style>


<div class="inline">
    <div>
      <img src="/img/IMG_20210531_151157-2-scaled.jpg" alt="Liam standing next to a bunch of tvs">
    </div>
  <h1>
    I like to work to supporting people at the intersection of creativity, learning, and communication by designing creative learning experiences, managing programs, and building relationships.
  </h1>
</div>




<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Design')" id="defaultOpen">Design</button>
  <button class="tablinks" onclick="openTab(event, 'Learning Communities')">Learning Communities</button>
  <button class="tablinks" onclick="openTab(event, 'Facilitation')">Facilitation</button>
</div>

<div id="Design" class="tabcontent">
  <p>Design for playful learning means making “objects to think with.”Blocks create a playable interface with gravity for toddlers that are building their first mental models of the world. My design work builds on building blocks to create playable interfaces with complex ideas.</p> <p>I make play materials and guidebooks that empower people to make creative choices and learn through playful exploration.</p>
</div>

<div id="Learning Communities" class="tabcontent">
  <p>All communities, be they workplaces or makerspaces, are learning communities; but they’re not created equal. The culture of every community can evolve to be more participatory, equitable, playful, and creative. I have worked with many organizations to create tools and cultivate a culture of learning and cooperation.</p> 
</div>

<div id="Facilitation" class="tabcontent">
  <p>The 21st century is collaborative. Don’t preach at; play with.
I design and facilitate workshops and events that give people a context to play and explore new tools and mediums. Play promotes deeper learning, strengthening social ties, and stimulates creative thinking.</p>
</div>

## Recent and upcoming workshops and talks

**Playful Learning and Sustainable Energy | Cambridge MA | July 7-8 2023**  
\- Guest MC

**[Playful Schools Conference](https://learningthroughplay.com/about-us/events/playful-schools-conference/) | Broadcast | March 28 2023**  
\- Workshop: Playing Together at a Distance

**[Reinventing Learning](https://reinventlearning.org/) | Boulder CO | 14-17 Oct 2022**  
\- Workshop: Gameshifting

**[Playful Schools Conference](https://learningthroughplay.com/about-us/events/playful-schools-conference/) | Online | 10 Feb 2022**  
\- Workshop: The Pedagogy of Karaoke, Ironic Armor in Introductory Experiences

**[Experimenting, Experiencing, Reflecting](https://www.eer.info/) | Copenhagen, DK | 1 Sep 2021**  
\- Workshop: Playing with the Sun w/ Amos Blanton

**[NEXT Library Conference](http://nextlibrary) | Aarhus, DK | Jun 2021**  
\- Workshop: Creative learning through tinkering with analogue video equipment

**Dokk1 Creative Learning Research Group | Aarhus, DK | May 2021**  
\- Workshop: Stop Animation Microworlds with TinkerQube

**[Wonderful Idea Co. World Tour](https://www.indiegogo.com/projects/wico-presents-a-tinkering-world-tour#/) | Online | May 2021**  
\- Talk: Presentation on outdoor tinkering

**Computer Clubhouse | Online | Mar 2021**  
\- Workshop: Creating and animating self portraits with prized objects (with the Tinkering Studio and Lifelong Kindergarten)



<script>
function openTab(evt, tabName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.className += " active";
}

document.getElementById("defaultOpen").click();

</script>