# Τεκμηριώνουμε τον κώδικά μας

- Το DocBlock χρησιμεύει ως inline documentation.
- Βελτιώνει το code completion σε IDE όπως το [PhpStorm](https://www.jetbrains.com/phpstorm).
- Μετατρέπεται αυτόματα σε API documentation, π.χ.&nbsp;[phpDocumentor](http://www.phpdoc.org).

```php
/**
 * Track a shipment by voucher number.
 *
 * @param  string $voucher                 A voucher number formatted as `PS123456789GR`
 * @return \Illuminate\Support\Collection  List of all the shipment steps
 *
 * @throws \LaravelGreece\Courier\CourierException  If the voucher number is invalid
 *
 * @license MIT
 */
public function track($voucher) {
  // ...
}
```
