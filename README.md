# Swoft Captcha

A Captcha Library that Imitation from thinkphp Captcha developed for swoft. 

## Usage

Build a captcha in controller
```php
/**
 * @RequestMapping("/")
 */
public function index(Response $response): Response
{
    $captcha = new Captcha();

    return $captcha->entry($response);
}
```

Check if the captcha code is correct
```PHP
$captcha = new Captcha();

return $captcha->check($code);
```
