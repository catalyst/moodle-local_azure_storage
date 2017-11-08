# Azure Storage SDK - Moodle Plugin

A moodle plugin containing the Microsoft Azure Storage SDK for PHP.

To use the SDK, simply include the autoloader contained within this plugin.

```php
require_once($CFG->dirroot . '/local/azure_storage/vendor/autoload.php');
```

## Why does this exist? ##

There is a growing collection of various moodle plugins that require these Azure libraries in order to work.
We don't want to have multiple copies of these libraries bundled into each plugin, firstly because they
are quite large, but also because it can cause issues with library namespaces and php auto loading.

Plugins that depend on this library are:

https://github.com/catalyst/moodle-tool_objectfs


## Supported Moodle Versions

This plugin requires Moodle 2.6+

## Installation

You can install this plugin from the plugin directory or get the latest version
on GitHub.

```bash
git clone https://github.com/catalyst/moodle-local_azure_storage local/azure_storage
```

# Crafted by Catalyst IT


This plugin was developed by Catalyst IT Australia:

https://www.catalyst-au.net/

![Catalyst IT](/pix/catalyst-logo.png?raw=true)


# Contributing and Support

Issues, and pull requests using github are welcome and encouraged! 

https://github.com/catalyst/moodle-local_azure_storage/issues

If you would like commercial support or would like to sponsor additional improvements
to this plugin please contact us:

https://www.catalyst-au.net/contact-us
