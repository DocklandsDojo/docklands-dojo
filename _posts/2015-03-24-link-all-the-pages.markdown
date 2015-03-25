---
layout: post
title:  "Link all the pages"
date:   2015-03-24 20:21:49
categories: my-first-website
step: 6
---


We're going to add links to all the pages we've created. This will allow us to navigate from one page to another no matter where we are in the site. Right now, the only links we have are on the index.html Home page.

To do this we'll open up the index.html file in our editor, copy the HTML code for the links and then paste it into the other files (`about-me.html`, `games.html`, `family.html` and so on). We'll also add a link back to the Home page.

###Step 1
Open `index.html` in your editor and select the HTML code for the links.

<img src="{{site.baseurl}}/assets/link-the-pages.png" width="80%" />


To select the code for the links:

* click just before the ul opening tag
* keep the mouse or touchpad button pressed down and then drag down, highlighting the text as you go
* take your finger off the button when you get to the ul closing tag


###Step 2
When the links are selected, check that you’ve included ALL of the start and end tags for the `ul`, then copy this text (`Edit` > `Copy`)

###Step 3
Open one of the web pages you made earlier (let's use the About Me page (`about-me.html`).

###Step 4
Click just before the `h1` opening tag and paste the links (`Edit` > `Paste`)

You should end up with this —
<img src="{{site.baseurl}}/assets/links-about-me.png" width="80%" />

Can you see where the links have been pasted?

###Step 6
Save `about-me.html` and open it in your browser. You can see that the links appear above the `h1` element.
They look a bit strange however. It would be better if they ran across the top in a row like the top menu bar you see on most web sites.

_We'll do that on the next Card._

Before we do though, can you do two things?

1. Add a link to the Home page above the About Me link.
2. Then copy the full set of links to all the other pages (except the Home page as it already has them).

Put the links in the same place before the `h1` element.

<a href="{{site.baseurl}}{% post_url 2015-03-24-style-the-menu %}" class="btn next-step pull-right">Next Step: Style the menu</a>
