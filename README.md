# Hugo JS Libraries

A small collection of JS libraries that works well with Hugo, packaged and ready for use as Hugo Modules. 

Hugo has great support for [JavaScript building](https://gohugo.io/hugo-pipes/js/), but these libraries stand solid on their own and you don't need `npm` to use them. It's similar to including the libraries from CDN, but you get the added benefit of:

* Offline use.
* They are aware of the Hugo life cycle (minify, fingerprint, add integrity hash only when in production).
* The dependencies can be vendored (`hugo mod vendor`) to make your site truly standalone.
* ...


See each component's README for usage.

## Versioning

These modules have their own semver versioning scheme that does not match the upstream library they wrap. To see the current upstream versions, use:

```bash
hugo mod graph
```

To update one module:

```
hugo mod get -u github.com/gohugoio/hugo-mod-jslibs/instantpage
```

To update all:

```
hugo mod get -u
```

The Hugo documentation has more information about [Hugo Modules](https://gohugo.io/hugo-modules/), how versioning works etc.
