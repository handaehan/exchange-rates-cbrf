# PHP Class ExchangeRatesCBRF

## Requirements
1. PHP 5 or greater
2. SOAP and SimpleXML

## Installation

Install via Composer
```sh
composer require thalidzhokov/exchange-rates-cbrf
```

OR include _ExchangeRatesCBRF.php_ in your PHP code
```php
require_once("ExchangeRatesCBRF.php");
```

## Usage
Examples of using ExchangeRatesCBRF Class to get exchange rates of the Central Bank of Russia


__Example 1__ \
Get exchange rate of Ukrainian Hryvnia (Alphabetic currency code - UAH) on 25.05.2015
```php
$rates = new ExchangeRatesCBRF("2015-05-25");
echo $rates->GetRate("UAH");
```

__Example 2__ \
Get cross-rate of the US Dollar to Euro on 26.06.2015
```php
$rates = new ExchangeRatesCBRF("2015-06-26");
echo $rates->GetCrossRate("EUR", "USD");
```

__Example 3__ \
Get exchange rates of the Central Bank of Russia on 27.07.2015 
```php
$rates = new ExchangeRatesCBRF("2015-07-27");
echo $rates->GetRates();
```
