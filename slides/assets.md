# Assets

```php
public function boot()
{
    $this->publishes([
        __DIR__.'/path/to/assets' => public_path('vendor/courier'),
    ], 'public');
}
```

```html
<link href="{{ asset('vendor/courier/track.css') }}">
```
