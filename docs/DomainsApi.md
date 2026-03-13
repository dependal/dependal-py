# dependal.DomainsApi

All URIs are relative to *https://api.dependal.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**check_tenant_domain**](DomainsApi.md#check_tenant_domain) | **POST** /v1/tenant/domains/{domain}/check | Check tenant domain verification
[**create_tenant_domain**](DomainsApi.md#create_tenant_domain) | **POST** /v1/tenant/domains | Add tenant domain
[**get_tenant_domain**](DomainsApi.md#get_tenant_domain) | **GET** /v1/tenant/domains/{domain} | Get tenant domain details
[**list_tenant_domains**](DomainsApi.md#list_tenant_domains) | **GET** /v1/tenant/domains | List tenant domains


# **check_tenant_domain**
> TenantDomainCheckResponse check_tenant_domain(domain)

Check tenant domain verification

Re-checks the verification status of a tenant domain and returns the latest provider verification state.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.tenant_domain_check_response import TenantDomainCheckResponse
from dependal.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dependal.com
# See configuration.py for a list of all supported configuration parameters.
configuration = dependal.Configuration(
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
with dependal.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = dependal.DomainsApi(api_client)
    domain = 'domain_example' # str | Domain name to check

    try:
        # Check tenant domain verification
        api_response = api_instance.check_tenant_domain(domain)
        print("The response of DomainsApi->check_tenant_domain:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->check_tenant_domain: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **str**| Domain name to check | 

### Return type

[**TenantDomainCheckResponse**](TenantDomainCheckResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Domain verification status |  -  |
**401** | Missing or invalid credentials |  -  |
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_tenant_domain**
> TenantDomainCreateResponse create_tenant_domain(tenant_domain_create_request)

Add tenant domain

Registers a domain for the authenticated tenant and begins the verification process.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.tenant_domain_create_request import TenantDomainCreateRequest
from dependal.models.tenant_domain_create_response import TenantDomainCreateResponse
from dependal.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dependal.com
# See configuration.py for a list of all supported configuration parameters.
configuration = dependal.Configuration(
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
with dependal.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = dependal.DomainsApi(api_client)
    tenant_domain_create_request = {"domain":"yourdomain.com"} # TenantDomainCreateRequest | 

    try:
        # Add tenant domain
        api_response = api_instance.create_tenant_domain(tenant_domain_create_request)
        print("The response of DomainsApi->create_tenant_domain:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->create_tenant_domain: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenant_domain_create_request** | [**TenantDomainCreateRequest**](TenantDomainCreateRequest.md)|  | 

### Return type

[**TenantDomainCreateResponse**](TenantDomainCreateResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Domain created |  -  |
**400** | Request validation failed |  -  |
**401** | Missing or invalid credentials |  -  |
**409** | Conflict |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_tenant_domain**
> TenantDomainDetailResponse get_tenant_domain(domain)

Get tenant domain details

Returns details for a tenant domain, including SES verification status and required DNS records.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.tenant_domain_detail_response import TenantDomainDetailResponse
from dependal.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dependal.com
# See configuration.py for a list of all supported configuration parameters.
configuration = dependal.Configuration(
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
with dependal.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = dependal.DomainsApi(api_client)
    domain = 'domain_example' # str | Domain name to retrieve

    try:
        # Get tenant domain details
        api_response = api_instance.get_tenant_domain(domain)
        print("The response of DomainsApi->get_tenant_domain:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->get_tenant_domain: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **str**| Domain name to retrieve | 

### Return type

[**TenantDomainDetailResponse**](TenantDomainDetailResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Tenant domain details |  -  |
**401** | Missing or invalid credentials |  -  |
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_tenant_domains**
> TenantDomainsResponse list_tenant_domains()

List tenant domains

Returns the domains registered for the authenticated tenant.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.tenant_domains_response import TenantDomainsResponse
from dependal.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.dependal.com
# See configuration.py for a list of all supported configuration parameters.
configuration = dependal.Configuration(
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
with dependal.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = dependal.DomainsApi(api_client)

    try:
        # List tenant domains
        api_response = api_instance.list_tenant_domains()
        print("The response of DomainsApi->list_tenant_domains:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DomainsApi->list_tenant_domains: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**TenantDomainsResponse**](TenantDomainsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Tenant domains |  -  |
**401** | Missing or invalid credentials |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

