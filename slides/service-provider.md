# Service Provider

- Αντιστοιχεί κλάσεις και dependencies στον service&nbsp;container.
- Φορτώνει αρχεία όπως views, configurations, localizations, migrations, routes, κ.α.

```php
namespace LaravelGreece\Courier;

use GuzzleHttp\Client;
use Illuminate\Support\ServiceProvider;

class CourierServiceProvider extends ServiceProvider
{
    public function register()
    {
        $this->app->singleton(Elta::class, function ($app) {
            $client = new Client(['base_uri' => 'http://www.elta-courier.gr']);

            return new Elta($client);
        });
    }
}
```
