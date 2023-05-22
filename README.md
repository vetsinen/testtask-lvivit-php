# testtask-lvivit-php

Write a simple PHP library for the Laravel framework.
This library should allow us to get all DNS records for the specified domain name.

## Acceptance  criteria:

### Required
* Application should use the latest PHP version
* Application should use "composer" to install all dependencies
* Application should use be compatible with latest Laravel framework
* Application should have unit tests
* The final result should be posted on GitHub and should have comments with a clear message about what was done there

### Not required
* Application should have README instructions on how to setup this library

### Example
```php
$result = $coolDNSService->getDnsRecords("gmail.com");

print_r($result);

[
    ["type" => "A", "name" => "gmail.com", "ttl" => "3360", "data" => "142.250.1.19"],
    ["type" => "TXT", "name" => "gmail.com", "ttl" => "18640", "data" => "globalsign-smime-dv=CDYX+XFHUw2wml6/Gb8+59BsH31KzUr6c1l2BPvqKX8="],
    ...
];
```
