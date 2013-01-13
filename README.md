# ZURB Foundation Bundle for Symfony2

## Current Version

Foundation v3.2.3

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "bmatzner/foundation-bundle": "*"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Bmatzner\FoundationBundle\BmatznerFoundationBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update bmatzner/foundation-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<link rel="stylesheet" type="text/css" href="{{ asset('bundles/bmatznerfoundation/css/foundation.min.css') }}" />
<script type="text/javascript" src="{{ asset('bundles/bmatznerfoundation/js/foundation.min.js') }}"></script>
```

If you require the special Modernizr build included with Foundation's sample apps, refer to the bmatzner/modernizr-bundle
which this bundle also requires

## Licenses

Refer to the source code of the included files for license information

## References

1. http://foundation.zurb.com
2. http://symfony.com