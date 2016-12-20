# Migrations

```php
public function boot()
{
    $this->loadMigrationsFrom(__DIR__.'/path/to/migrations');
}
```

```bash
$ php artisan migrate
```
