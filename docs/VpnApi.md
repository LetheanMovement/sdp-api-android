# VpnApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**startLetheand**](VpnApi.md#startLetheand) | **GET** /letheand/start | 



## startLetheand

> startLetheand(dataDir, version)



### Example

```java
// Import classes:
//import org.lthn.sdp.api.VpnApi;

VpnApi apiInstance = new VpnApi();
String dataDir = null; // String | Returns the binary version
Boolean version = null; // Boolean | Returns the binary version
try {
    apiInstance.startLetheand(dataDir, version);
} catch (ApiException e) {
    System.err.println("Exception when calling VpnApi#startLetheand");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dataDir** | **String**| Returns the binary version | [default to null]
 **version** | **Boolean**| Returns the binary version | [optional] [default to null]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

