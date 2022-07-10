# HTTPFactory
PSR-17 HTTP Factory Library


## Requirements

- PHP 7.4 or higher
- PSR-17 HTTP Factory Package
- [InitPHP HTTP Library](https://github.com/InitPHP/HTTP) 

## Installation

```
composer require initphp/http-factory
```

## Usage

```php
require_once "vendor/autoload.php";
use InitPHP\HTTPFactory\HTTPFactory;

$http = new HTTPFactory();

$request = $http->createRequest('GET', 'https://www.muhammetsafak.com.tr');
```

## Credits

- [Muhammet ŞAFAK](https://www.muhammetsafak.com.tr) <<info@muhammetsafak.com.tr>>

## License

Copyright &copy; 2022 [MIT License](./LICENSE)
