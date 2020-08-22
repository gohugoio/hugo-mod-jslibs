# Hugo JS Libraries

A small collection of JS libraries that works well with Hugo, packaged and ready for use as Hugo Modules. 

Hugo has great support for [JavaScript building](https://gohugo.io/hugo-pipes/js/), but these libraries stand solid on their own and you don't need `npm` to use them. It's similar to including the libraries from CDN, but you get the added benefit of:

* Offline use.
* They are aware of the Hugo life cycle (minify, fingerprint, add integrity hash only when in production).
* The dependencies can be vendored (`hugo mod vendor`) to make your site truly standalone.
* ...

To use AlpineJS with Turbolinks you can just import the modules into your config and then add this to youer `head`

```
{{ partialCached "jslibs/alpinejs/script-src.html" "-" }}
{{ partialCached "jslibs/turbolinks/script-src.html" "-" }}
```

See each component's README for usage. The Hugo documentation has more information about [Hugo Modules](https://gohugo.io/hugo-modules/).

## Versioning

