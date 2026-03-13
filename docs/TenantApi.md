# openapi_client.TenantApi

All URIs are relative to *https://api.dependal.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accept_tenant_policies**](TenantApi.md#accept_tenant_policies) | **POST** /v1/tenant/policies/accept | Accept tenant policies


# **accept_tenant_policies**
> TenantPoliciesAcceptResponse accept_tenant_policies()

Accept tenant policies

Records acceptance of the current required policy version for the authenticated tenant.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import openapi_client
from openapi_client.models.tenant_policies_accept_response import TenantPoliciesAcceptResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dependal.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.dependal.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TenantApi(api_client)

    try:
        # Accept tenant policies
        api_response = api_instance.accept_tenant_policies()
        print("The response of TenantApi->accept_tenant_policies:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantApi->accept_tenant_policies: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**TenantPoliciesAcceptResponse**](TenantPoliciesAcceptResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Policies accepted successfully |  -  |
**401** | Missing or invalid credentials |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

