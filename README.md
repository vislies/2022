---
layout: blank
---
# Template for VisLies web pages

This repository contains the template for the VisLies web pages. This is
the starting point for each year.

## Installing Jekyll

These pages use Jekyll for building the html, so the first thing you need
to do is have Jekyll installed on your machine. As of now, VisLies is being
hosted on GitHub pages, so Jekyll is run for you there, but you will surely
wish to also run Jekyll locally to preview pages.

Jekyll uses ruby, so first you need ruby installed on your system. Ruby
might already be installed on your system, but you might need a newer
version in order to be able to download the necessary packages. Generally,
you can use a package manager do the dirty work. For example, using
macports ruby can be installed with

``` sh
sudo port install ruby24
port select --set ruby ruby24
```

Next, you need to install bundler, which is done through the `gem`
installer part of ruby.

``` sh
sudo gem install bundler
```

Once bundler is installed you can finally (finally!) install Jekyll.

``` sh
sudo gem install jekyll
```

## Running Jekyll

Typically, the first thing you need to do when you want to build a specific
repository is to make sure that you have all the packages and plugins
necessary. To update Jekyll on local machine, be in this repositories root
directory and run:

``` sh
bundle install
```

You may need to run this with root perissions (i.e. `sudo`).

Once you have done this, you should be able to run the Jekyll server, which
will build the html pages and start a simple web server.

``` sh
bundle exec jekyll serve
```

## Updating the configuration

It is a good idea to occasionally update the "gems" used by Jekyll. When
starting a new configuration, consider running

``` sh
bundle update
```

This will upgrade the underlying Jekyll software. GitHub will likely
complain about security problems with older gems. After running the update,
you should then run `bundle install` again.

Get started with the web site by updating the `_config.yaml` configuration
file. The biggest need is to update the configuration to the current year.
Typically, the items needed to be updated are `title`, `email`, `baseurl`,
and `this-year`.

## Creating content

Content is created by editing the `.md` files in this repository. Every
`.md` file found in the repository will be converted to an html page. The
most likely pages to change are `index.md` and `gallery/index.md`. There
are templates for each of these pages. Take particular attention to the
configuration at the top of each one.

### Laying out images

The VisLies pages, particularly those of the galleries, typically have lots
of images, and usually these images can be clicked to get a larger image.
The typical markdown way of embedding an image is to use syntax like the
following:

``` markdown
![Alt text](path/to/image.png)
```

However, there are two problems with this. The first is that we want the
image to have a link to a higher resolution form of the image. The second
is that we often want to size or float these images to the "right" place.
We solve both of these problems by wrapping the image within an `<a>` html
tag. The tag will create the link to the full resolution image and define a
class that gives the position of the image.

``` markdown
<a href="foo.png" class="image-right">
![A foo](foo-thumbnail.png)
</a>
```

As you laying down images, it is a good idea to differentiate images that
lie from good examples. You can ensure that it is clear which images lie by
adding a "lie" image to them, this can be done by adding an `<img
src="lie.png" class="lie" />` tag.

``` markdown
<a href="foo.png" class="image-right">
<img src="lie.png" class="lie" />
![A foo](foo-thumbnail.png)
</a>
```

The CSS for the VisLies pages have the following classes to help position
images:

  * `image-left` Floats the image to the left of the text.
  * `image-right` Floats the image to the right of the text.
  * `image-full` Stretches the image across the entire page.
  * `image-half` Sizes the image to half the width of the text. Put 2
    images together when using `image-half`.
  * `image-third` Sizes the image to a third the width of the text. Put 3
    images together when using `image-third`.

Two of these class, `image-right` and `image-left`, create floating image,
and they are used a lot. One of the problems with floating images is that
they can run too far into other text and create issues. The easiest way to
get around this is to create a `div` tag that acts as a barrier that only
continues the page after the bottom of any active float. This can be done
simply by making a `div` tag with the class `image-stop` where you want to
stop the float's affect.

``` markdown
<a href="foo.png" class="image-right">
![A foo](foo-thumbnail.png)
</a>

Here is a small amount of text referring to this image.

<div class="image-stop" />
```

If the text contained with the `div` does not go all the way to the bottom
of the image, whitespace will be added to fill that space. Perhaps not the
most elegant solution, but it works well enough.

## Making the site live

To make the site live, you first have to create a repository in GitHub's
`vislies` group named with the current year. Push the previously created
repository there.

Next, go to the GitHub project's setting page and find the `GutHub Pages`
options near the bottom. Change the `Source` to the branch with the pages
to post (probably `main`). Once you do that, you should see a green box
that says your site is published at `https://www.vislies.org/20XX` (with
the appropriate year substituted).

When the site is ready to become the default landing, update the
redirection in the [vislies.github.io] repository to point to the new site.

[vislies.github.io]: https://github.com/vislies/vislies.github.io

## Link to gallery

When you first create the site, you won't have a gallery (because the event
has not happened yet). When you are ready to add the gallery, edit the
`_config.yaml` file and change the `gallery-ready` item from `false` to
`true`.
