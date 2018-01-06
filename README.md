BinBag—an alternative Composer repository (BETA)
================================================

<img align="right" src="/img/piles-of-garbage.jpg">

[BinBag](https://binbag.github.io) is a [Composer](https://getcomposer.org)
repository, established to host useful packages that may not be deemed
suitable for inclusion in the default [Packagist](https://packagist.org/)
repository.

The initial aim of the project is to enable the installation of PHAR and
non-PHP binaries using Composer, although its scope may expand in future.

Usage
-----

Visit [binbag.github.io](https://binbag.github.io) to explore the list of
hosted packages.

Add the repository definition to your project's `composer.json` file:

```json
{
    "repositories": [
        {
            "type": "composer",
            "url": "https://binbag.github.io"
        }
    ]
}
```

Then simply add desired package specifcations to the `require` or `require-dev`
section of the file.

Contributing
------------

Packages can be contributed by adding a "package" repository type entry to the
`repositories` section of the [`satis.json`](./satis.json) file. Submit a pull
request to have the contribution reviewed.

Caveat Utilitor
---------------

This repository enables the installation of software provided by third-parties,
not connected with, or warranted by the repository's maintainers. Users install
the software at their own risk.

--
Powered by [Satis](https://github.com/composer/satis) •
Hosted on GitHub Pages •
Maintained by [j13k](https://github.com/j13k)
