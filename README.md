# HTTPFactory

> ## ⚠️ DEPRECATED — Use [`initphp/http`](https://github.com/InitPHP/HTTP) instead
>
> As part of the InitPHP package consolidation, **this package has been merged into [`initphp/http`](https://github.com/InitPHP/HTTP) starting with version 2.2.** The consolidated package ships its own PSR-17 factory under `\InitPHP\HTTP\Factory\Factory`.
>
> This repository is kept read-only for historical reference. **No further updates will be released.**
>
> ### Why this package no longer works
>
> `\InitPHP\HTTPFactory\HTTPFactory` was written against `initphp/http:^1.x`, which used the flat `\InitPHP\HTTP\*` namespace. In `initphp/http:^2.0` those classes moved to `\InitPHP\HTTP\Message\*`, so this package's `use` statements no longer resolve.
>
> ### Migration
>
> ```diff
> - "initphp/http-factory": "^1.0",
> - "initphp/http": "^1.0",
> + "initphp/http": "^2.2"
> ```
>
> Your existing imports keep working: `initphp/http:^2.2` ships a `class_alias` so `\InitPHP\HTTPFactory\HTTPFactory` remains resolvable. Composer also declares a `replace` for this package, so the two will not be installed side-by-side.
>
> When you next touch the code, prefer the canonical class:
>
> ```php
> // Before
> use InitPHP\HTTPFactory\HTTPFactory;
> $factory = new HTTPFactory();
>
> // After
> use InitPHP\HTTP\Factory\Factory;
> $factory = new Factory();
> ```

---

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
