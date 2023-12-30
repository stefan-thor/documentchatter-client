# Swagger\Client\DefaultApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addDocumentDocumentPost**](DefaultApi.md#adddocumentdocumentpost) | **POST** /document/ | Add Document
[**addIndexIndexPost**](DefaultApi.md#addindexindexpost) | **POST** /index/ | Add Index
[**askDocumentAskPost**](DefaultApi.md#askdocumentaskpost) | **POST** /ask/ | Ask Document
[**askDocumentMcqPost**](DefaultApi.md#askdocumentmcqpost) | **POST** /mcq/ | Ask Document

# **addDocumentDocumentPost**
> addDocumentDocumentPost($body)

Add Document

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: APIKeyHeader
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\DocumentRequestSchema(); // \Swagger\Client\Model\DocumentRequestSchema | 

try {
    $apiInstance->addDocumentDocumentPost($body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->addDocumentDocumentPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\DocumentRequestSchema**](../Model/DocumentRequestSchema.md)|  |

### Return type

void (empty response body)

### Authorization

[APIKeyHeader](../../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **addIndexIndexPost**
> \Swagger\Client\Model\IndexResponseSchema addIndexIndexPost($body)

Add Index

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: APIKeyHeader
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\IndexSchema(); // \Swagger\Client\Model\IndexSchema | 

try {
    $result = $apiInstance->addIndexIndexPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->addIndexIndexPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\IndexSchema**](../Model/IndexSchema.md)|  |

### Return type

[**\Swagger\Client\Model\IndexResponseSchema**](../Model/IndexResponseSchema.md)

### Authorization

[APIKeyHeader](../../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **askDocumentAskPost**
> \Swagger\Client\Model\QuestionSchema askDocumentAskPost($body)

Ask Document

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: APIKeyHeader
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\QuestionSchema(); // \Swagger\Client\Model\QuestionSchema | 

try {
    $result = $apiInstance->askDocumentAskPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->askDocumentAskPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\QuestionSchema**](../Model/QuestionSchema.md)|  |

### Return type

[**\Swagger\Client\Model\QuestionSchema**](../Model/QuestionSchema.md)

### Authorization

[APIKeyHeader](../../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **askDocumentMcqPost**
> \Swagger\Client\Model\MCQSchema askDocumentMcqPost($body)

Ask Document

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: APIKeyHeader
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\MCQSchema(); // \Swagger\Client\Model\MCQSchema | 

try {
    $result = $apiInstance->askDocumentMcqPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->askDocumentMcqPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\MCQSchema**](../Model/MCQSchema.md)|  |

### Return type

[**\Swagger\Client\Model\MCQSchema**](../Model/MCQSchema.md)

### Authorization

[APIKeyHeader](../../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

