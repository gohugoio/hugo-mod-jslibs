## Description

This module wraps [AlpineJS](https://github.com/alpinejs/alpine).

This module also packages [Alpine Turbolinks Adapter](https://github.com/SimoTod/alpine-turbolinks-adapter) by [@SimoTod](https://github.com/SimoTod).

## Installation

First, add the module import to your site or theme component's configuration's module section:

```toml
[module]
[[imports]]
path = "github.com/gohugoio/hugo-mod-jslibs/alpinejs/v3"
```

To use `v2` of AlpineJS, use the module path `github.com/gohugoio/hugo-mod-jslibs/alpinejs`

Then add the script source in the head section of your template (typically in the `baseof.html`):


```html
<head>
{{ partialCached "jslibs/alpinejs/v3/script-src.html" "-" }}
</head>
```



