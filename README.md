# Popcorn.js Bundle for Symfony2

## Current Version

Popcorn.js 1.3

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "bmatzner/popcorn-bundle": "*"
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
        new Bmatzner\PopcornBundle\BmatznerPopcornBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update bmatzner/popcorn-bundle
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
<script type="text/javascript" src="{{ asset('bundles/bmatznerpopcorn/js/popcorn-complete.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://popcornjs.org/
2. http://symfony.com
