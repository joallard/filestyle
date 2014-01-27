Filestyle
=========
**Filestyle** is a lightweight jQuery plugin to make file upload styling easy.

It allows you to use a text button or an image for your file field.

Usage
-----
Mark your file upload field with the `filestyle` class:

```html
<input type="file" class="filestyle" id="user_image" />
```

Include `jquery.filestyle.js` as a script (depends on jQuery):

```html
<script src="/js/jquery.filestyle.js"></script>
```

And the plugin auto-magically activates to give you a styleable field!

```html
<div class="filestyle container">
  <input class="file filestyle file-name" readonly="" tabindex="999" />
  <div class="file-button">
    Choose a file
    <input type="file" id="user_image" class="filestyle" />
  </div>
</div>
```

### Manual activation (without class)

You can also activate it manually via Javascript:

```js
$("input[type=file]").filestyle()
```

Data attributes
---------------
You can set text and class individually with *data* attributes put on the file field:

* `data-button-class`: Button class
* `data-button-text`: Button text

These will have priority over the options passed to `$.fn.filestyle()`.


Options
-------
* `buttonText` (default: `"Choose File"`):
    The text you want the button to display.

* `buttonClass` (default: `'file-button'`):
    The class of the button with the text.

* `tabIndex` (default: `false`):
    The [tab index][tabindex] of the button.

* `fileSelected(filename)`:
    A callback for when the file field is changed. It will be called
    with the file name.

[tabindex]: https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#tabindex


Authors and Licence
-------------------
This plugin was originally made by Mika Tuupola ([@tuupola][@tuupola]).

Since then, Matt Pegler ([@pegler][@pegler]) has pitched in, as I
([@joallard][@joallard]).

It is subject to the [MIT Licence][MIT].

[@joallard]: https://github.com/joallard
[@pegler]: https://github.com/pegler
[@tuupola]: https://github.com/tuupola
[MIT]: http://opensource.org/licenses/MIT
