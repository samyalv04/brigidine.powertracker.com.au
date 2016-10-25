ColorBox Gallery Dir
====================

Popup gallery from images using `jQuery Colorbox`

* list
* dir

## Config

Need to add JS and CSS to front matter - either on the page or to the site

```yaml
javascript:
  - /js/jquery.colorbox.js
```

## List

```html
<div class="col-xs-12">
    {% assign gallery = page.gallery %}
    {% include colorbox/list.html %}
</div>
```

We define the images in the front matter

```yaml
gallery:
  - path: gallery/open.jpg
  - path: gallery/closed.jpg
  - path: gallery/this.jpg
  - path: gallery/that.jpg
```

## Directory

Each image will be shown in alphabetical order.

```html
<div class="col-xs-12">
    {% assign gallerybase = page.dir %}
    {% include colorbox/dir.html %}
</div>
```

## To do

```
{% include footer.html param="value" variable-param=page.variable %}
```
