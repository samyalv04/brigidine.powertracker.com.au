Form Helper Includes
--------------------

Include these components to build forms to set up a Bootstrap form item

## Config

Assign the Notify JS to the page or site front maatter

```yaml
javascript:
- /js/verify.notify.min.js

```


## RadioBox

```yaml
filename:
    id: isocertified
    required: true
    label: What label to display?
    items:
        - Yes
        - No
```

```html
{% assign formradiogroup = page.fieldname %}
{% include form\radiogroup.html %}
```
