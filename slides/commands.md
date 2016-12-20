# Commands

```php
public function boot()
{
    if ($this->app->runningInConsole()) {
        $this->commands([
            CourierTrackingCommand::class,
        ]);
    }
}
```

```bash
$ php artisan courier:track
```
