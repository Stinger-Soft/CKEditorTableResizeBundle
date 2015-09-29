# CKEditor plugin Table Resize Bundle for Symfony2
Symfony2 Bundle to integrate the CKEditor plugin Table Resize

## Current Version

Table Resize v4.5.3

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/ckeditor-tableresize-bundle": "~4.5.3"
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
        new Stinger\CKEditorTableResizeBundle\StingerCKEditorTableResizeBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/ckeditor-tableresize-bundle
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

### Usage

``` yaml
trsteel_ckeditor:
    external_plugins:
      tableresize:
        path: 'bundles/stingerckeditortableresize'
```



# Licenses

Refer to the source code of the included files for license information

# References

1. http://ckeditor.com/addon/tableresize
2. http://symfony.com