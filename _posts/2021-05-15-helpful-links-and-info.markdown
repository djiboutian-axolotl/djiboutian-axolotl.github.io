---
layout: post
title:  "Helpful notes for using Jekyll."
date:   2021-05-15 07:15:11 -0400
categories: blog
use_math: false
author: Your Correspondent
---

This post will including an ever-updating list of helpful Jekyll- and markdown-related notes.

## Jekyll commands

I can type `bundle info --path minima` to get the gem installation location.

To test locally, type `bundle exec jekyll serve`.

Edit from mobile? Check!

* Endash: &ndash; `&ndash;`
* Emdash: &mdash; `&mdash;`
* Minus: &minus; `&minus;`

## Links in markdown
1. Standard links in which both the label and URL are defined together:
  `[label](http://example.com)`
1. Reference links, which can be in one of two forms:
  `[label][key] or [key]`
  `[key]: http://example.com`
1. Automatic links, where the label is the URL:
  `<http://example.com>`

## Images

The following instructions are helpful for adding an image to a post.

### Center and caption an image
I can center and caption  an image with the following code:
{% highlight html %}
<figure class="align-center">
 <p align="center">
  <img src="/images/image_name.png" alt="alt text">
 </p>
 <figcaption>
  <p align="center">
   <i>My caption.</i>
  </p>
 </figcaption>
</figure> 
{% endhighlight %}

### Remove background from image
I used <https://www.remove.bg/> to remove the image's background.

### Remove metadata from image
To remove metadata from the image, I did the following:
1. Right click on the image
1. Select **Properties**, then **Details**
1. Click **Remove Properties and Personal Information**
1. Click **Create a copy with all possible properties removed** in the top of the window
1. Click **OK**

The newly created image now has all metadata removed!
