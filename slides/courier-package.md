# Courier package

- Αναζήτηση αποστολής ΕΛ.ΤΑ. μέσω voucher

```php
namespace LaravelGreece\Courier;

use GuzzleHttp\ClientInterface;

class Elta
{
    protected $client;

    public function __construct(ClientInterface $client)
    {
        $this->client = $client;
    }

    public function track($voucher)
    {
        $response = $this->client->post('track.php', [
            'form_params' => ['number' => $voucher],
        ]);

        return json_decode($response->getBody());
    }
}
```
