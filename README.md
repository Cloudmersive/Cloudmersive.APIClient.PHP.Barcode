# cloudmersive_barcode_api_client
Barcode APIs let you generate barcode images, and recognize values from images of barcodes.

[Cloudmersive Barcode API](https://www.cloudmersive.com/barcode-api) provides advanced barcode generation, lookup and recognition capabilities.

- API version: v1
- Package version: 1.4.5


## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/cloudmersive/cloudmersive_barcode_api_client.git"
    }
  ],
  "require": {
    "cloudmersive/cloudmersive_barcode_api_client": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/cloudmersive_barcode_api_client/vendor/autoload.php');
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

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\BarcodeLookupApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = "value_example"; // string | Barcode value

try {
    $result = $apiInstance->barcodeLookupEanLookup($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BarcodeLookupApi->barcodeLookupEanLookup: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://api.cloudmersive.com*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BarcodeLookupApi* | [**barcodeLookupEanLookup**](docs/Api/BarcodeLookupApi.md#barcodelookupeanlookup) | **POST** /barcode/lookup/ean | Lookup a barcode value and return product data
*BarcodeScanApi* | [**barcodeScanImage**](docs/Api/BarcodeScanApi.md#barcodescanimage) | **POST** /barcode/scan/image | Scan an image for a barcode and turn the result.  Supported barcode types include AZTEC, CODABAR, CODE_39, CODE_93, CODE_128, DATA_MATRIX, EAN_8, EAN_13, ITF, MAXICODE, PDF_417, QR_CODE, RSS_14, RSS_EXPANDED, UPC_A, UPC_E, All_1D, UPC_EAN_EXTENSION, MSI, PLESSEY, IMB
*GenerateBarcodeApi* | [**generateBarcodeEAN13**](docs/Api/GenerateBarcodeApi.md#generatebarcodeean13) | **POST** /barcode/generate/ean-13 | Validates and generate a EAN-13 barcode as a PNG file, a type of 1D barcode
*GenerateBarcodeApi* | [**generateBarcodeEAN8**](docs/Api/GenerateBarcodeApi.md#generatebarcodeean8) | **POST** /barcode/generate/ean-8 | Validates and generate a EAN-8 barcode as a PNG file, a type of 1D barcode
*GenerateBarcodeApi* | [**generateBarcodeQRCode**](docs/Api/GenerateBarcodeApi.md#generatebarcodeqrcode) | **POST** /barcode/generate/qrcode | Generate a QR code barcode as a PNG file, a type of 2D barcode which can encode free-form text information
*GenerateBarcodeApi* | [**generateBarcodeUPCA**](docs/Api/GenerateBarcodeApi.md#generatebarcodeupca) | **POST** /barcode/generate/upc-a | Validate and generate a UPC-A barcode as a PNG file, a type of 1D barcode
*GenerateBarcodeApi* | [**generateBarcodeUPCE**](docs/Api/GenerateBarcodeApi.md#generatebarcodeupce) | **POST** /barcode/generate/upc-e | Validates and generate a UPC-E barcode as a PNG file, a type of 1D barcode


## Documentation For Models

 - [BarcodeLookupResponse](docs/Model/BarcodeLookupResponse.md)
 - [BarcodeScanResult](docs/Model/BarcodeScanResult.md)
 - [ProductMatch](docs/Model/ProductMatch.md)


## Documentation For Authorization


## Apikey

- **Type**: API key
- **API key parameter name**: Apikey
- **Location**: HTTP header


## Author




