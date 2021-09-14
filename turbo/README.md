## Description

This module wraps [Turbo](https://github.com/hotwired/turbo).

## Installation

First, add the module import to your site or theme component's configuration's module section:

```toml
[module]
[[imports]]
path = "github.com/gohugoio/hugo-mod-jslibs/turbo"
```

Then add the script source in the head section of your template (typically in the `baseof.html`):


```html
<head>
{{ partialCached "jslibs/turbo/script-src.html" "-" }}
</head>
```

Note that the target `src` folder gets mounted to `assets/jslibs/turbo`.