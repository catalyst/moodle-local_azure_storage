Azure Storage SDK - Moodle Plugin
==================================

To update the contents of this plugin.

* execute `composer update`
* git add -f vendor
* update the version details in version.php
* update the version details in thirdpartylibs.xml

For Moodle 4.2+
=======================
Moodle 4.2 includes GuzzleHttp in core, and is a higher version with breaking API changes. Additional steps are required to re-namespace the guzzle included here to maintain parallel compatibility.

1. Replace all `*.php` files `GuzzleHttp` with `GuzzleHttpLocal`
2. In `vendor/composer/autoload_psr4.php` modify the `GuzzleHttp` keys in the class map array, and change them to be `GuzzleHttpLocal`