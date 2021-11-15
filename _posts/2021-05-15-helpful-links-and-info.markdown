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

## How to make posts

To make posts, I follow the following strategy.

### Header for the post

I put something like this at the top of my post, and then I type the remainder of the post below it. (The text provided below is the header that I used to create this post.)

{% highlight markdown %}
---
layout: post
title:  "Helpful notes for using Jekyll."
date:   2021-05-15 07:15:11 -0400
categories: blog
use_math: false
author: Your Correspondent
---
{% endhighlight %}

Note that setting the `use_math` parameter to `True` loads some stuff to allow us to write equations in a Latex style. If you do not use math in your post, leave the parameter as `False` so that the post will load more quickly.

### Titling a post

A post should be titled in the format `YYYY-MM-DD-title-of-post.markdown`. For example, this post is named `2021-05-15-welcome-to-jekyll.markdown`.

### Publishing a post

When a post is ready to be published, open the program "Git Bash" (I have it installed -- I'm a little shaky on what the setup process was for this). Make sure you are in the correct directory. For me, the correct directory is `~/OneDrive/Desktop/GitHub-Pages/djiboutian-axolotl.github.io`.

Next, type `git add .` so that the newest post is added to the GitHub repo. Then, type `git commit -am "summary of this commit"` (where you replace *summary of this commit* with your own summary; this summary should be placed in quotes). Finally, type `git push`. After a minute or two, the post should appear on your website!



