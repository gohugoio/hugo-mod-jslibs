
For AlpineJS >= v3, see https://github.com/gohugoio/hugo-mod-jslibs-dist/tree/main/alpinejs

## Description

This module wraps [AlpineJS](https://github.com/alpinejs/alpine).

This module also packages [Alpine Turbolinks Adapter](https://github.com/SimoTod/alpine-turbolinks-adapter) by [@SimoTod](https://github.com/SimoTod).

## Installation

First, add the module import to your site or theme component's configuration's module section:

```toml
[module]
[[imports]]
path = "github.com/gohugoio/hugo-mod-jslibs/alpinejs"
```

Then add the script source in the head section of your template (typically in the `baseof.html`):


```html
<head>
{{ partialCached "jslibs/alpinejs/script-src.html" "-" }}
</head>
```

Note, if used with Turbolinks, the order matters:

```html
{{ partialCached "jslibs/alpinejs/script-src.html" "-" }}
{{ partialCached "jslibs/turbolinks/script-src.html" "-" }}
```

