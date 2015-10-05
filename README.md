jQuery PageSlide
================

PageSlide is a jQuery plugin which slides a webpage over to reveal an
additional interaction pane.

Demo
----

There are a couple of examples included with this package. Or, if you
can’t wait to download it, see it live on the [responsive demo] or
[original project page].

Options
-------

### speed

The speed at which the page slides over. Accepts standard jQuery effects
speeds (e.g. ‘fast’, ‘normal’ or milliseconds). (default=200)

### direction

Which direction does the page slide? Accepts ‘left’ or ‘right’.
(default=‘right’)

### modal

By default, when pageslide opens, you can click on the document to close
it. If modal is set to ‘true’, then you must explicitly close PageSlide
using \$.pageslide.close(); (default=false)

### iframe

By default, linked pages are loaded into an iframe. Set this to false if
you don’t want an iframe. (default=true)

### href

Override the source of the content. Optional in most cases, but required
when opening pageslide programmatically (e.g. <code>\$.pageslide({ href:
‘\#some-element’ });</code> ) (default=null)

Setup
-----

### CommonJS / AMD

```bash
npm i jquery-pageslide --save
```


```js
// CommonJS
var jQuery = require('jquery');
require('jquery-pageslide')(jQuery);

// AMD
define(['jquery', 'jquery-pageslide'], function (jQuery, pageslide) {
  pageslide(jQuery)
})
```

### In the HEAD tag:

Ideally, near the bottom of the page.

To use, call pageslide on an <code><a></code> tag that either links to a
page or an anchor of a hidden element.

        $('a').pageslide();

Or, open pageslide programatically:

        $.pageslide({ href: '#some-element' });
        $.pageslide({ href: 'some-page.html' });

To close pageslide programatically:

        $.pageslide.close();

Changelog
---------

### Version 2.0

-   Completely rewritten
-   Externalized CSS
-   Content loaded into an iframe

### Version 1.3

-   Older versions of PageSlide are located in this repository, however
    if you would like to contribute to the original plugin’s
    development, please use contributor [Derek Perez’s repository].

Support
-------

Basic support is offered through Github’s issues tracker. Many requests
are resolved through the help of fellow PageSlide users and myself,
however assistance is not guaranteed or timely.

If you are in need of immediate support, or would like customizations to
the script, [Premium Support] is available for \$17. Premium Support
provides you with direct email access to me, and allows me to set time
aside to hel

  [responsive demo]: http://srobbin.github.com/jquery-pageslide
  [original project page]: http://srobbin.com/blog/jquery-pageslide/
  [Derek Perez’s repository]: https://github.com/perezd/jquery-pageslide
  [Premium Support]: https://www.paypal.com/cgi-bin/webscr?business=scott@halobrite.com&cmd=_xclick&currency_code=USD&amount=17&item_name=jQuery%20PageSlide%20Premium%20Support