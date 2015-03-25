---
layout: post
title:  "Add Some Style"
date:   2015-03-24 20:18:49
categories: my-first-website
step: 5
---


The `index.html` Home page looks a bit boring.
You can change its appearance using a `CSS file`.

<img src="{{site.baseurl}}/assets/a-little-style.png" width="80%" />


A CSS file contains the recipe for how the web page should appear.
It's a separate file from the HTML file and it’s linked to the HTML file like this:

{% highlight html %}
<link type="text/css" rel="stylesheet" href="css/simple.css"/>
{% endhighlight %}

###Step 1
Open the index.html file in your editor, and locate the above link

What this link is telling you is that the appearance of the page is controlled by a stylesheet named `simple.css` which is located in the `css` folder.

###Step 2
Go into the css folder and locate `simple.css`. Create a duplicate copy, and name it `home.css`

###Step 3
Now change the link in the `index.html` file so that it is pointing to `home.css`

{% highlight html %}
<link type="text/css" rel="stylesheet" href="css/home.css"/>
{% endhighlight %}

###Step 4
Save `index.html` and open it in your browser. Note that `home.css` contains just one statement:

{% highlight css %}
body {
  font-family: sans-serif;
}
{% endhighlight %}

This statement is called a `selector` and it tells the browser how to format everything inside the `body` element of the HTML file. What this selector is saying is _set everything in the body element in a sans-serif font_.


###Step 5
Modify the body selector by adding a rule to include a background image, and add a new selector which says how to format the `h1` element. So the finished `home.css` file will look like this

{% highlight css %}
body {
  font-family: sans-serif;
  background-image: url('../images/cool-lee.png');
}
h1 {
  padding: 0.5em;
  background-color: black;
  color: white;
  border-radius: 0.5em;
}
{% endhighlight %}



###Step 6
Add the rules one at a time, saving as you go. Click refresh in your browser each time you add a new rule so that you understand the difference the new rule makes.

>Notice how the selectors contain a number of individual formatting rules. Each rule is ended by a semi-colon (`;`) and consists of a property (such as color) followed by a colon (`:`) and then a value (such as `white`). Notice, also, that rules are enclosed in curly braces (`{` and `}`).

<a href="{{site.baseurl}}{% post_url 2015-03-24-link-all-the-pages %}" class="btn next-step pull-right">Next Step: Link all the pages</a>

