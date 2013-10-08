Filestyle
=========
**Filestyle** is a lightweight plugin to make file upload styling easy.

Usage
-----
Insert your file upload field as you normally would:

```html
<input type="file" id="user_image" />
```

Include `jquery.filestyle.js` as a script (depends on jQuery):

```html
<script src="/js/jquery.filestyle.js"></script>
```

Activate it on the fields you want to style:

```js
$("input[type=file]").filestyle()
```

And there you go.

Options
-------
* `buttonText` (default: `"Choose File"`): 
    The text you want the button to display.

* `buttonClass` (default: `'fileButton'`):
    The class of the button with the text.

* `tabIndex` (default: `false`):
    The [tab index][tabindex] of the button.

* `fileSelected(filename)`:
    A callback for when the file field is changed. It will be called
    with the file name.

[tabindex]: https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#tabindex

Data attributes
---------------
You can also set things individually with *data* attributes put on the file field:

* `data-button-class`: Button class
* `data-button-text`: Button text

These will have priority over the options passed to `$.fn.filestyle()`.

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
