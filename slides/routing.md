# Routing

```php
public function boot()
{
    $this->loadRoutesFrom(__DIR__.'/path/to/routes.php');
}
```

```html
<a href="{{ route('courier.track', $voucher) }}">Αναζήτηση αποστολής</a>
```
