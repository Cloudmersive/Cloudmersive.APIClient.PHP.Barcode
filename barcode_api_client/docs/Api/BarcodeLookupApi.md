# barcode_api_client_invoke\BarcodeLookupApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**barcodeLookupEanLookup**](BarcodeLookupApi.md#barcodeLookupEanLookup) | **POST** /barcode/lookup/ean | Lookup a barcode value and return product data


# **barcodeLookupEanLookup**
> \barcode_api_client_invoke\barcode_api_client_model\BarcodeLookupResponse barcodeLookupEanLookup($value)

Lookup a barcode value and return product data

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = barcode_api_client_invoke\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = barcode_api_client_invoke\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new barcode_api_client_invoke\Api\BarcodeLookupApi(
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | **string**| Barcode value |

### Return type

[**\barcode_api_client_invoke\barcode_api_client_model\BarcodeLookupResponse**](../Model/BarcodeLookupResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json, application/xml, text/xml

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

