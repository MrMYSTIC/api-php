# UnoEuro PHP API #

## Description ##

This package provides a PHP interface to the [UnoEuro REST API](https://www.unoeuro.com/docs/api.php).

## Install via Composer ##

We recommend installing this package with [Composer](http://getcomposer.org/).

### Download Composer ###

To download Composer, run in the root directory of your project:

```bash
curl -sS https://getcomposer.org/installer | php
```

You should now have the file `composer.phar` in your project directory.

### Install Dependencies ###

Run in your project root:

```
php composer.phar require unoeuro/api-php
```

### Require Autoloader ###

After installing the dependencies, you need to require the Composer autoloader
from your code:

```php
require 'vendor/autoload.php';
```

## Usage  ##

```php
require 'vendor/autoload.php';
$unoeuro = new UnoEuro\Client('account', 'apikey');
$products = $unoeuro->get('my/products/');
var_dump($products);
```


## Contributing ##

Please submit pull requests, we love you <3
