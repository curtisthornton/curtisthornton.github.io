---
layout: post
title:  "Big Texas Containers Analysis"
image: /
color: 004080
---
*This is an official analysis of [bigtexascontainers.com](http://www.bigtexascontainers.com) and any branding associated with the parent company.*

---

# Initial Inspection
Upon first loading the site, we are presented with a bit of a mess. There is a lot of content that seems important, but nothing stands out against everything else, making it more of a wall of text than anything worthwhile (although I'm sure it is).

There is also a lot of images with text embedded into them. That's not good, either for SEO or the site in general.

The site feels cold and unwelcoming from its stiff use of tables and default typography. Even scrolling down from the main page, I already feel lost as it is dificult to decipher what exactly the website is trying to tell me.

It's also confusing that some images are repeated and some of the text is hard to read because they are inside images. The big "Like Us on Facebook" reminds the user that this is a very web 1.0 website.

# Coding
Okay, where to start.

There is way too much coding going on the main page for what is being loaded, and that's mostly because it looks to be built by a WYSIWYG editor. There are a ton of empty \<div\> and \<font\> frames.

I am also seeing a lot of inline CSS, which is a *major* problem, since inline CSS should only be used as a last resort and as a temporary solution to a styling problem. I have no doubt that whatever program was used to build this site injected them.

Since everything was build using tables, the site is not mobile-friendly. Many elements are mis-aligned from this as well.


