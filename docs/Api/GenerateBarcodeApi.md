# Swagger\Client\GenerateBarcodeApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generateBarcodeCode128**](GenerateBarcodeApi.md#generateBarcodeCode128) | **POST** /barcode/generate/code-128 | Generate a EAN-13 code barcode as PNG file
[**generateBarcodeEAN13**](GenerateBarcodeApi.md#generateBarcodeEAN13) | **POST** /barcode/generate/ean-13 | Generate a EAN-13 code barcode as PNG file
[**generateBarcodeEAN8**](GenerateBarcodeApi.md#generateBarcodeEAN8) | **POST** /barcode/generate/ean-8 | Generate a EAN-8 code barcode as PNG file
[**generateBarcodeQRCode**](GenerateBarcodeApi.md#generateBarcodeQRCode) | **POST** /barcode/generate/qrcode | Generate a QR code barcode as PNG file
[**generateBarcodeUPCA**](GenerateBarcodeApi.md#generateBarcodeUPCA) | **POST** /barcode/generate/upc-a | Generate a UPC-A code barcode as PNG file
[**generateBarcodeUPCE**](GenerateBarcodeApi.md#generateBarcodeUPCE) | **POST** /barcode/generate/upc-e | Generate a UPC-E code barcode as PNG file


# **generateBarcodeCode128**
> string generateBarcodeCode128($value, $width, $height, $include_label)

Generate a EAN-13 code barcode as PNG file

Validates and generate a EAN-13 barcode as a PNG file, a type of 1D barcode

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\GenerateBarcodeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = "value_example"; // string | Barcode value to generate from
$width = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$height = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$include_label = true; // bool | Optional: show text label on the image of the barcode value, default is true.

try {
    $result = $apiInstance->generateBarcodeCode128($value, $width, $height, $include_label);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GenerateBarcodeApi->generateBarcodeCode128: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | **string**| Barcode value to generate from |
 **width** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **height** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **include_label** | **bool**| Optional: show text label on the image of the barcode value, default is true. | [optional]

### Return type

**string**

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/octet-stream

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **generateBarcodeEAN13**
> string generateBarcodeEAN13($value, $width, $height, $include_label)

Generate a EAN-13 code barcode as PNG file

Validates and generate a EAN-13 barcode as a PNG file, a type of 1D barcode

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\GenerateBarcodeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = "value_example"; // string | Barcode value to generate from
$width = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$height = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$include_label = true; // bool | Optional: show text label on the image of the barcode value, default is true.

try {
    $result = $apiInstance->generateBarcodeEAN13($value, $width, $height, $include_label);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GenerateBarcodeApi->generateBarcodeEAN13: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | **string**| Barcode value to generate from |
 **width** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **height** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **include_label** | **bool**| Optional: show text label on the image of the barcode value, default is true. | [optional]

### Return type

**string**

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/octet-stream

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **generateBarcodeEAN8**
> string generateBarcodeEAN8($value, $width, $height, $include_label)

Generate a EAN-8 code barcode as PNG file

Validates and generate a EAN-8 barcode as a PNG file, a type of 1D barcode

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\GenerateBarcodeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = "value_example"; // string | Barcode value to generate from
$width = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$height = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$include_label = true; // bool | Optional: show text label on the image of the barcode value, default is true.

try {
    $result = $apiInstance->generateBarcodeEAN8($value, $width, $height, $include_label);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GenerateBarcodeApi->generateBarcodeEAN8: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | **string**| Barcode value to generate from |
 **width** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **height** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **include_label** | **bool**| Optional: show text label on the image of the barcode value, default is true. | [optional]

### Return type

**string**

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/octet-stream

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **generateBarcodeQRCode**
> string generateBarcodeQRCode($value, $width, $height)

Generate a QR code barcode as PNG file

Generate a QR code barcode as a PNG file, a type of 2D barcode which can encode free-form text information

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\GenerateBarcodeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = "value_example"; // string | QR code text to convert into the QR code barcode
$width = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$height = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.

try {
    $result = $apiInstance->generateBarcodeQRCode($value, $width, $height);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GenerateBarcodeApi->generateBarcodeQRCode: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | **string**| QR code text to convert into the QR code barcode |
 **width** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **height** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]

### Return type

**string**

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/octet-stream

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **generateBarcodeUPCA**
> string generateBarcodeUPCA($value, $width, $height, $include_label)

Generate a UPC-A code barcode as PNG file

Validate and generate a UPC-A barcode as a PNG file, a type of 1D barcode

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\GenerateBarcodeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = "value_example"; // string | UPC-A barcode value to generate from
$width = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$height = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$include_label = true; // bool | Optional: show text label on the image of the barcode value, default is true.

try {
    $result = $apiInstance->generateBarcodeUPCA($value, $width, $height, $include_label);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GenerateBarcodeApi->generateBarcodeUPCA: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | **string**| UPC-A barcode value to generate from |
 **width** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **height** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **include_label** | **bool**| Optional: show text label on the image of the barcode value, default is true. | [optional]

### Return type

**string**

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/octet-stream

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **generateBarcodeUPCE**
> string generateBarcodeUPCE($value, $width, $height, $include_label)

Generate a UPC-E code barcode as PNG file

Validates and generate a UPC-E barcode as a PNG file, a type of 1D barcode

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\GenerateBarcodeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = "value_example"; // string | UPC-E barcode value to generate from
$width = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$height = 56; // int | Optional: width of the barcode in pixels.  Minimum value of 10.
$include_label = true; // bool | Optional: show text label on the image of the barcode value, default is true.

try {
    $result = $apiInstance->generateBarcodeUPCE($value, $width, $height, $include_label);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GenerateBarcodeApi->generateBarcodeUPCE: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | **string**| UPC-E barcode value to generate from |
 **width** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **height** | **int**| Optional: width of the barcode in pixels.  Minimum value of 10. | [optional]
 **include_label** | **bool**| Optional: show text label on the image of the barcode value, default is true. | [optional]

### Return type

**string**

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/octet-stream

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

