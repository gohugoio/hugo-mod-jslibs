## Installation

First, add the module import to your site or theme component's configuration's module section:

```toml
[module]
[[imports]]
path = "github.com/gohugoio/hugo-mod-jslibs/instantpage"
```

Then add the script source before the end body tag:


```html
<body>
...
{{ partialCached "jslibs/instantpage/script-src.html" "-" }}
</body>
```

See the [instant.page](https://instant.page/) documentation for configuration.