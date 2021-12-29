# This is a service plugin used to generate url

[![Latest Stable Version](http://poser.pugx.org/felipemateus/http-build-url/v)](https://packagist.org/packages/felipemateus/http-build-url) [![Total Downloads](http://poser.pugx.org/felipemateus/http-build-url/downloads)](https://packagist.org/packages/felipemateus/http-build-url) [![Latest Unstable Version](http://poser.pugx.org/felipemateus/http-build-url/v/unstable)](https://packagist.org/packages/felipemateus/http-build-url) [![License](http://poser.pugx.org/felipemateus/http-build-url/license)](https://packagist.org/packages/felipemateus/http-build-url) [![PHP Version Require](http://poser.pugx.org/felipemateus/http-build-url/require/php)](https://packagist.org/packages/felipemateus/http-build-url)

This package implements a function which allows you to create urls with user and password parameter from http.

## Instalation

```bash
composer require felipemateus/http-build-url
```

## Example

```php
require_once __DIR__ . '/vendor/autoload.php'; 

$url = http_build_url("http://example.com",
            array(
                "user" => "teste",
                "pass" => "teste",
            )
        );

print($url);
// https://teste:teste@example.com

```

### Url parts

scheme
user
pass
host
port
path
query
fragment
