# Image thumbnailing plugin for Jekyll

Generates a thumbnail to an image (at an exact resolution, maintaining aspect
ratio) and renders an image tag.

## This fork

This is a fork of the original project at
https://github.com/mrdanadams/jekyll-thumbnailer with the following changes:

  * Removes Octopress support
  * Fixes to allow thumbnail generation when non-default build destination is
    configured
  * Resizes to an exact dimension maintaining aspect ratio (centre gravity,
    changes canvas size)
  * Adds width/height into img tag

## Usage

```
{% thumbnail /path/to/local/image.png 50x50 %}
```

The dimensions will be given directly to imagemagick.
See http://www.imagemagick.org/Magick++/Geometry.html.

## Installation

* add the gem: `gem "mini_magick"` (and `bundle install`)
* copy thumbnail.rb to plugins folder
* start thumbnailing

