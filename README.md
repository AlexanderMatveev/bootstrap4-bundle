Bootstrap 4 bundle for Symfony 3+
=======================

## Current Version

Bootstrap 4.0.0

## Installation

``` bash

composer require alexandermatveev/bootstrap4-bundle

```

### Add bundle to your application kernel (Symfony 3)

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new AlexanderMatveev\Bootstrap4Bundle\AlexanderMatveevBootstrap4Bundle(),
        // ...
    );
}
```

### Install assets (Symfony 3)

Given your server's public directory is named "web", install the public vendor resources

``` bash
bin/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
bin/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<link href="{{ asset('bundles/alexandermatveevbootstrap4/lib/css/bootstrap.min.css') }}" rel="stylesheet">
<script type="text/javascript" src="{{ asset('bundles/alexandermatveevbootstrap4/lib/js/bootstrap.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. https://getbootstrap.com
2. http://symfony.com

