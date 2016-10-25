jQuery Flexslider
-----------------

* `list` needs a list provided
* 'dir' needs a path provided

## Config

* add `flexlisder` to the SASS list in `/css/style.css`
* add `jquery.flexslider.min.js` to `javascript` includes
* define the banners variable
* include the file

```yaml
javascript:
- /js/jquery.flexslider.min.js
```


## List

In this example, the banners are in banners directory. These need to be defined
as a list in the front matter

```yaml
banners:
- url: "banners/image1.jpg"
- url: "banners/image2.jpg"
- url: "banners/image3.jpg"
```

And then used in the HTML

```html
{% assign flexslider = page.banners %}
{% include flexslider\list.html %}
```

This could be wrapped in a DIV

```html
<div class="container">
    <div class="row">
        <div class="col-xs-12">
            {% assign flexslider = page.banners %}
            {% include flexslider.html %}
        </div>
    </div>
</div>
```

## Dir

* coming...