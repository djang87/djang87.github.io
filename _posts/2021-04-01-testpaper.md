---
title:  Test Paper.
tags:
  - Friday Theme
  - HTMLaaaaa
  - Image Gallery
---

Haha. Here's an example for multiple images that uses Bootstrap's Carousel javascript component for a photo slideshow. You don't need to write any JavaScript, just place some Liquid tags and HTML in your Markdown.

<!--more-->

To automate the layout, a list of images is stored in a frontmatter variable. The post then loops over that list to output the carousel. This is easier than copy-pasting the same HTML for each image.

Here's the carousel in action.

<div id="carouselExampleControls" class="carousel slide mb-4" data-ride="carousel">
    <div class="carousel-inner">
        {% for img in page.images %}
            <div class="carousel-item {% if forloop.first %}active{% endif %}">
                <img src="{{ img }}" class="d-block w-100" alt="">
            </div>
        {% endfor %}
    </div>
    <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
    </a>
</div>

(The photos are from [Unsplash](http://www.unsplash.com)!)

To create this, put a list of image URLs in your page's front matter, like this:

{% highlight yaml %}
{% raw %}

images:
  - http://www.something.com/path/to/image1.jpg
  - http://www.something.com/path/to/image2.jpg
  - http://www.something.com/path/to/image3.jpg

{% endraw %}
{% endhighlight %}

And then add the following block of HTML:

{% highlight html %}
{% raw %}

<div id="carouselExampleControls" class="carousel slide mb-4" data-ride="carousel">
    <div class="carousel-inner">
        {% for img in page.images %}
            <div class="carousel-item {% if forloop.first %}active{% endif %}">
                <img src="{{ img }}" class="d-block w-100" alt="">
            </div>
        {% endfor %}
    </div>
    <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
    </a>
</div>

{% endraw %}
{% endhighlight %}

You could extend this idea by combining it with a modal to show the carousel in fullscreen mode.
