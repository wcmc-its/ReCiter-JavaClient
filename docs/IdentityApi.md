# IdentityApi

All URIs are relative to *http://wcmc-its-reciter-service.us-west-2.elasticbeanstalk.com/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addIdentity**](IdentityApi.md#addIdentity) | **POST** /identity | Add a new Identity
[**deleteIdentity**](IdentityApi.md#deleteIdentity) | **DELETE** /identity/{uid} | Deletes an Identity
[**getIdentityyId**](IdentityApi.md#getIdentityyId) | **GET** /identity/{uid} | Find Identity by ID
[**updateIdentity**](IdentityApi.md#updateIdentity) | **PUT** /identity | Update an existing Identity


<a name="addIdentity"></a>
# **addIdentity**
> addIdentity(body)

Add a new Identity



### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.IdentityApi;


IdentityApi apiInstance = new IdentityApi();
Identity body = new Identity(); // Identity | Identity object that needs to be added
try {
    apiInstance.addIdentity(body);
} catch (ApiException e) {
    System.err.println("Exception when calling IdentityApi#addIdentity");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Identity**](Identity.md)| Identity object that needs to be added |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteIdentity"></a>
# **deleteIdentity**
> deleteIdentity(uid)

Deletes an Identity



### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.IdentityApi;


IdentityApi apiInstance = new IdentityApi();
Long uid = 789L; // Long | Identity id to delete
try {
    apiInstance.deleteIdentity(uid);
} catch (ApiException e) {
    System.err.println("Exception when calling IdentityApi#deleteIdentity");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uid** | **Long**| Identity id to delete |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getIdentityyId"></a>
# **getIdentityyId**
> Identity getIdentityyId(uid)

Find Identity by ID

Returns a single Identity

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.IdentityApi;


IdentityApi apiInstance = new IdentityApi();
Long uid = 789L; // Long | ID of pet to return
try {
    Identity result = apiInstance.getIdentityyId(uid);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling IdentityApi#getIdentityyId");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uid** | **Long**| ID of pet to return |

### Return type

[**Identity**](Identity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateIdentity"></a>
# **updateIdentity**
> updateIdentity(body)

Update an existing Identity



### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.IdentityApi;


IdentityApi apiInstance = new IdentityApi();
Identity body = new Identity(); // Identity | Identity object that needs to be added
try {
    apiInstance.updateIdentity(body);
} catch (ApiException e) {
    System.err.println("Exception when calling IdentityApi#updateIdentity");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Identity**](Identity.md)| Identity object that needs to be added |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

