---
layout: post
title:  "Style the menu links"
date:   2015-03-24 20:24:49
categories: my-first-website
step: 8
---



<img src="{{site.baseurl}}/assets/style-menu-links.png" width="100%" />

To style to your links like those above you’ll need to edit the HTML files and the CSS file.

###Step 1
In each of your HTML files remove the one link from the menu that leads to same page. For example, in the `about-me.html` page you will remove:

{% highlight html %}
<a href="about-me.html">
{% endhighlight %}

link, in the `games.html` page you will remove

{% highlight html %}
<a href="games.html">
{% endhighlight %}

<img src="{{site.baseurl}}/assets/style-menu-links-1.png" width="100%" />

Do this for all the files in your site (for example family.html and pets.html). Notice that after you make this change the menu entry is no longer clickable.


###Step 2
Add a `class` attribute with a value of `selected` to the same `li` elements.

<img src="{{site.baseurl}}/assets/style-menu-links-2.png" width="100%" />

This doesn’t do anything on its own (refresh in the browser and the menu still looks the same). BUT, adding the class attribute allows you to pick out the link in the CSS file and colour it yellow. Here’s how!

<img src="{{site.baseurl}}/assets/style-menu-links-3.png" width="100%" />


###Step 3

Refresh and you’ll see the selected link change to yellow. What you’ve done is added a new rule which applies only to `li` elements with a `class` attribute of `selected`. Notice the syntax in the CSS file — instead of specifying `li` in the rule, you specify `li.selected`


###Step 4

 Remove the underline from the menu links:

<img src="{{site.baseurl}}/assets/style-menu-links-4.png" width="100%" />


###Step 5
Make the links light-blue and show the underline when you hover over them by adding a new rule to the CSS. This rule defines what will happen when you hover over an a element.

{% highlight css %}
ul li a:hover {
  color: #99DDFF;
  text-decoration: underline;
}
{% endhighlight %}


Note that `#99DDFF` is the code for the light-blue colour.


####That's it for today!