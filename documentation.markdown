---
layout: page
title: "Documentation"
weight: 2
---

## Blog Like a Hacker, In Style.

Byron is a theme for [Jekyll](https://github.com/mojombo/jekyll). It is based off of one of our latest [premium themes](byron.stylehatch.co) for tumblr at [Stylehatch](http://stylehatch.co/). We're big fans of Jekyll and the open source community, so we are trying something new.

![Byron Demo]({% if site.baseurl %}{{ site.baseurl }}{% endif %}/images/byron-demo-stage.png)

When we set out to create Byron we had long-form writings, essays and beautiful photography in mind.  Every post type has been thoughtfully crafted to create one Style Hatch’s most versatile premium themes yet. 

## Installation

Setting up this theme is fairly simple, but if you aren't already familiar with Jekyll take some time to read through their [documentation](http://jekyllrb.com/docs/home/).

- Install Jekyll: `gem install jekyll`
- Fork this repository
- Clone it: `git clone https://github.com/YOUR-USER/byron`
- Run the Jekyll server: `jekyll serve`

You should have a server up and running locally at <http://localhost:4000>.

[More on basic usage](http://jekyllrb.com/docs/usage/)

## Customization

Next you'll want to change a few things. Most of them can be changed directly in
[_config.yml](#). That's where we'll pull your name, Twitter username, color variables, and things like that.

There's a few other places that you'll want to change, too:

- [CNAME](#): If you're using
  this on GitHub Pages with a custom domain name, you'll want to change this
  to be the domain you're going to use. All that should be in here is a
  domain name on the first line and nothing else (like: `example.com`).
- [favicon.ico](#): This
  is a smaller version of my gravatar for use as the icon in your browser's
  address bar. You should change it to whatever you'd like.
- [apple-touch-icon.png](#):
  Again, this is my gravatar, and it shows up in iOS and various other apps
  that use this file as an "icon" for your site.

For custom CSS, there is an included override.css file for that purpose.

## Adding Posts
There are currently 5 supported post types in this theme. These are defined in the posts YAML front-matter using the variable `type: `

These types affect how the post is rendered. Some post types have extra post specific front-matter like `photo_url` or `link`. You can see how they work in the example posts for each type.

#### Text
Example YAML front-matter for this post type:
{% highlight yaml %}
---
layout: post
title: Blog Like a Hacker, In Style
category: posts
type: text
---
{% endhighlight %}

#### Photo
Example YAML front-matter for this post type:
{% highlight yaml %}
---
layout: post
title: Photos Look Great
category: posts
type: photo
photo_url: http://muke.me/images/mikeyzagprint.jpg
camera: Pentax K200D
apeture: f/11.0
exposure: 1/180
focal_length: 300mm
---
{% endhighlight %}

#### Embed
Example YAML front-matter for this post type:
{% highlight yaml %}
---
layout: post
title: Magnetic Magic
category: posts
type: embed
embed_code: <iframe src="http://player.vimeo.com/video/63773788?portrait=0&amp;badge=0" width="500" height="281" frameborder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>
---
{% endhighlight %}

#### Quote
Example YAML front-matter for this post type:
{% highlight yaml %}
---
layout: post
title: You're Only Paranoid Until It's True
category: posts
type: quote
source: unknown
---
{% endhighlight %}

#### Link
Example YAML front-matter for this post type:
{% highlight yaml %}
---
layout: post
title: Jonathan Moore
category: posts
type: link
link: http://jonathanmoore.com/
---
{% endhighlight %}

These are mostly specifc to the Byron Jekyll theme. See the Jekyll documentation for [more on adding posts](http://jekyllrb.com/docs/posts/).

## Creating Pages
All HTML or Markdown files with YAML front-matter will be parsed as individual pages separate from posts. In order to get these to show up in the main navigation they will need the following YAML front-matter.

{% highlight yaml %}
---
layout: page
title: your title
weight: 3
---
{% endhighlight %}

Weight is used to determine the order within the navigation items (1-10).

[More on creating pages](http://jekyllrb.com/docs/pages/)

## Deployment

You should deploy with [GitHub Pages](http://pages.github.com)- it's just
easier.

All you should have to do is rename your repository on GitHub to be `username.github.io`. Content from the master branch of your repository will be used to build and publish the GitHub Pages site, so make sure your Jekyll site is stored there.

If you're using it for a Project Page, create a new branch named `gh-pages`. The content of this branch will be rendered using Jekyll, and the output will become available under a subpath of your user pages subdomain, such as `username.github.io/project`

For more, see the Jekyll's documentation on [deploying to GitHub Pages](http://jekyllrb.com/docs/github-pages/) as well as [other deployment methods](http://jekyllrb.com/docs/deployment-methods/).

## Licensing

## Thanks

All icons are from Entypo pictograms by Daniel Bruce — [www.entypo.com](www.entypo.com)

Shout out to [@holman](https://twitter.com/holman) for the great example of how to build a nice Jekyll theme like he's done with [Left](https://github.com/holman/left).
