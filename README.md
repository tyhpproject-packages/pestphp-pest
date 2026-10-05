<!-- tyhp-readme:start -->
# tyhpdef/pestphp-pest

Tyhp type definitions for `pestphp/pest` `4.7.8`.

```bash
composer require --dev tyhpdef/pestphp-pest:4.7.8
```

This is a metapackage. Composer also installs `tyhpdef/pestphp-pest-impl` (type files).
Require **this** name, not `tyhpdef/pestphp-pest-impl`.

See https://tyhplang.com.

## Maintain `pestphp/pest`? Ship the types yourself

If you are a Packagist maintainer of `pestphp/pest`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/pestphp-pest-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `pestphp/pest` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/pestphp-pest": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `pestphp/pest` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `pestphp/pest` with a real constraint,
   `"replace": { "tyhpdef/pestphp-pest": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `pestphp/pest` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/pestphp-pest` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
