## Installation

First, add the module import to your site or theme component's configuration's module section:

```toml
[module]
[[imports]]
path = "github.com/gohugoio/hugo-mod-jslibs/instantclick"
```

Then add the script source before the end body tag:


```html
<body>
...
{{ partialCached "jslibs/instantclick/script-src.html" "-" }}
</body>
```

The dafault init script looks like this:

```js
// Default init script for InstantClick.
InstantClick.init();

```

To do custom initialization, add a custonm script to your project in `assets/jslibs/instantclick/init.js`.

See the [InstantClick](http://instantclick.io/) documentation for configuration.
