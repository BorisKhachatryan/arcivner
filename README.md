# arcivner


```shell
composer require barryvdh/laravel-debugbar --dev
```

Laravel uses Package Auto-Discovery, so doesn't require you to manually add the ServiceProvider.

The Debugbar will be enabled when `APP_DEBUG` is `true`.

> If you use a catch-all/fallback route, make sure you load the Debugbar ServiceProvider before your own App ServiceProviders.

### Laravel without auto-discovery:

If you don't use auto-discovery, add the ServiceProvider to the providers array in config/app.php

```php
Barryvdh\Debugbar\ServiceProvider::class,
```