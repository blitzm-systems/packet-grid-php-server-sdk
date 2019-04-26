# OpenAPIClient-php
No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 1.0.0
- Build package: org.openapitools.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/OpenAPIClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Token
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\ClientTokenApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\CreateClientToken(); // \OpenAPI\Client\Model\CreateClientToken | the account id from the client side

try {
    $result = $apiInstance->createClientToken($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ClientTokenApi->createClientToken: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *http://http:/api*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ClientTokenApi* | [**createClientToken**](docs/Api/ClientTokenApi.md#createclienttoken) | **POST** /client-tokens/ | create a client token for a mobile device
*NotificationsApi* | [**send**](docs/Api/NotificationsApi.md#send) | **POST** /notifications/send/ | 


## Documentation For Models

 - [ClientToken](docs/Model/ClientToken.md)
 - [CreateClientToken](docs/Model/CreateClientToken.md)
 - [DispatchReport](docs/Model/DispatchReport.md)
 - [Error](docs/Model/Error.md)
 - [Notification](docs/Model/Notification.md)
 - [Recipient](docs/Model/Recipient.md)
 - [SendNotification](docs/Model/SendNotification.md)
 - [TransportEnum](docs/Model/TransportEnum.md)
 - [TransportReport](docs/Model/TransportReport.md)


## Documentation For Authorization


## Token

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header


## Author



