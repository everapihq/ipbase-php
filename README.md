<p align="center">
<img src="https://app.ipbase.com/img/logo/ipbase.png" width="300"/>
</p>

# ipbase-php - PHP IP data lookup

[![Latest Version on Packagist](https://img.shields.io/packagist/v/everapi/ipbase-php.svg?style=flat-square)](https://packagist.org/packages/everapi/ipbase-php)
[![Total Downloads](https://img.shields.io/packagist/dt/everapi/ipbase-php.svg?style=flat-square)](https://packagist.org/packages/everapi/ipbase-php)

This package is a PHP wrapper for [ipbase.com] that aims to make the usage of the API as easy as possible in your project.

## Installation

You can install the package via composer:

```bash
composer require everapi/ipbase-php
```

## Usage

Initialize the API with your API Key (get one for free at [ipbase.com]):

```php
$ipBase = new \Ipbase\Ipbase\IpbaseClient('YOUR-API-KEY');
```

Afterwards you can use the endpoints of the API like this:

```php
echo $ipBase->status();
```


```php
echo $ipBase->info([
    'ip' => '1.1.1.1',
    'language' => 'de',
]);
```


Learn more about endpoints, parameters and response data structure in the [docs].

[docs]: https://ipbase.com/docs
[ipbase.com]: https://ipbase.com

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
