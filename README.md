My Presentations
================

This is a collection of presentations that I have done/am going to do.  I am
hosting them here for ease of access and so people can take a look at how I
made this work with Jekyll (which I intend to explain in a minute).

All of the info found here is free for you to use and duplicate, and I only ask
for you to give me a little credit.  But if you don't, forget about it, this
most likely isn't ground breaking stuff here.


How these slides work with Jekyll
---------------------------------

To start, I am going to use Deck.js.  It's a solid framework for building a
slide show using HTML, but it uses css classes to differenciate between
different slides on a page.  This is fine except I wanted to use Markdown
because I don't really want to deal with HTML tags as little as possible.

Since I wanted find some way to do this, the best thing I could come up with
was to have each Jekyll "Post" be a slide and wrap them up in a single page.
The other thing I wanted was to be able to have more then one slide in a Repo.
To do this, I had to find some way to tell the difference between slides from
each slide show using just the basics of the Jekyll framework.

Jekyll has two things to work with that we can leverage to make this work:
categories and tags.  For me personally, I like catgories being the slide show,
and tags being the css tags that you can use to customize each individual
slide.  Honestly, you could flip flop the two, but like the tags to css tags
relationships.

What I do then is make a html page for each slideshow, and link it on the index
page.  For each presentation I do the following:

```HTML+Django
{% for slide in site.categories.SLIDE_CATEGORY %}
  <section class="slide" id="{{slide.categories.first}}">
    {{slide.content | markdownify}}
  </section>
{% endfor %}
```
This will create a slide portion for each slide.


Credit where credit is do
-------------------------

First off, there are obviously some tech's that need some credit here:

* [Jekyll](https://github.com/mojombo/jekyll):  Awesome blogging framework,
  nuff said.
* [Deck.js](https://github.com/imakewebthings/deck.js):  Awesome javascript/css
  slideshow framework, nuff said.

But while these technologies are great, I am don't really have the creative
juices to think of this all on my own.  So some credit should go to these
projects as well:

* [Patrick Byrne's Presentation pages](https://github.com/pbyrne/presentations):  
  The orignal idea for using github for hosting my presentations
* [Hekyll](https://github.com/bmcmurray/hekyll):  The original idea for using
  jekyll for this


License
-------
I am using the... oh who am I kidding, this isn't worth having a license...
