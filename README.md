<!-- tyhp-readme:start -->
# tyhpdef/symfony-expression-language

Tyhp type definitions for `symfony/expression-language` `7.4.18`.

```bash
composer require --dev tyhpdef/symfony-expression-language:7.4.18
```

This is a metapackage. Composer also installs `tyhpdef/symfony-expression-language-impl` (type files).
Require **this** name, not `tyhpdef/symfony-expression-language-impl`.

See https://tyhplang.com.

## Maintain `symfony/expression-language`? Ship the types yourself

If you are a Packagist maintainer of `symfony/expression-language`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-expression-language-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/expression-language` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-expression-language": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/expression-language` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/expression-language` with a real constraint,
   `"replace": { "tyhpdef/symfony-expression-language": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/expression-language` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-expression-language` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
