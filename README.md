<!-- tyhp-readme:start -->
# tyhpdef/hamcrest-hamcrest-php

Tyhp type definitions for `hamcrest/hamcrest-php` `3.0.0`.

```bash
composer require --dev tyhpdef/hamcrest-hamcrest-php:3.0.0
```

This is a metapackage. Composer also installs `tyhpdef/hamcrest-hamcrest-php-impl` (type files).
Require **this** name, not `tyhpdef/hamcrest-hamcrest-php-impl`.

See https://tyhplang.com.

## Maintain `hamcrest/hamcrest-php`? Ship the types yourself

If you are a Packagist maintainer of `hamcrest/hamcrest-php`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/hamcrest-hamcrest-php-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `hamcrest/hamcrest-php` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/hamcrest-hamcrest-php": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `hamcrest/hamcrest-php` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `hamcrest/hamcrest-php` with a real constraint,
   `"replace": { "tyhpdef/hamcrest-hamcrest-php": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `hamcrest/hamcrest-php` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/hamcrest-hamcrest-php` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
