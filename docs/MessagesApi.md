# dependal.MessagesApi

All URIs are relative to *https://api.dependal.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_message_status**](MessagesApi.md#get_message_status) | **GET** /v1/status/{messageId} | Get message delivery status
[**get_tenant_message**](MessagesApi.md#get_tenant_message) | **GET** /v1/tenant/messages/{messageId} | Get tenant message
[**list_tenant_message_events**](MessagesApi.md#list_tenant_message_events) | **GET** /v1/tenant/messages/{messageId}/events | List tenant message events
[**list_tenant_messages**](MessagesApi.md#list_tenant_messages) | **GET** /v1/tenant/messages | List tenant messages
[**send_email**](MessagesApi.md#send_email) | **POST** /v1/send | Send an email


# **get_message_status**
> MessageStatusResponse get_message_status(message_id)

Get message delivery status

Returns the current delivery status for a message.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.message_status_response import MessageStatusResponse
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
    api_instance = dependal.MessagesApi(api_client)
    message_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Get message delivery status
        api_response = api_instance.get_message_status(message_id)
        print("The response of MessagesApi->get_message_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessagesApi->get_message_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **UUID**|  | 

### Return type

[**MessageStatusResponse**](MessageStatusResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Message status |  -  |
**401** | Missing or invalid credentials |  -  |
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_tenant_message**
> TenantMessageResponse get_tenant_message(message_id)

Get tenant message

Returns a single message record for the authenticated tenant.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.tenant_message_response import TenantMessageResponse
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
    api_instance = dependal.MessagesApi(api_client)
    message_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | Message request ID

    try:
        # Get tenant message
        api_response = api_instance.get_tenant_message(message_id)
        print("The response of MessagesApi->get_tenant_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessagesApi->get_tenant_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **UUID**| Message request ID | 

### Return type

[**TenantMessageResponse**](TenantMessageResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Tenant message |  -  |
**401** | Missing or invalid credentials |  -  |
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_tenant_message_events**
> TenantMessageEventsResponse list_tenant_message_events(message_id, cursor=cursor, limit=limit)

List tenant message events

Returns the event timeline for a single tenant message, including internal processing events and provider delivery events.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.tenant_message_events_response import TenantMessageEventsResponse
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
    api_instance = dependal.MessagesApi(api_client)
    message_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | Message request ID
    cursor = 'cursor_example' # str | Opaque pagination cursor returned by a previous response (optional)
    limit = 50 # int | Maximum number of events to return (optional) (default to 50)

    try:
        # List tenant message events
        api_response = api_instance.list_tenant_message_events(message_id, cursor=cursor, limit=limit)
        print("The response of MessagesApi->list_tenant_message_events:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessagesApi->list_tenant_message_events: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **UUID**| Message request ID | 
 **cursor** | **str**| Opaque pagination cursor returned by a previous response | [optional] 
 **limit** | **int**| Maximum number of events to return | [optional] [default to 50]

### Return type

[**TenantMessageEventsResponse**](TenantMessageEventsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Message events |  -  |
**401** | Missing or invalid credentials |  -  |
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_tenant_messages**
> TenantMessagesResponse list_tenant_messages(cursor=cursor, limit=limit)

List tenant messages

Returns paginated message logs for the authenticated tenant.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.tenant_messages_response import TenantMessagesResponse
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
    api_instance = dependal.MessagesApi(api_client)
    cursor = 'cursor_example' # str | Opaque pagination cursor returned by a previous response (optional)
    limit = 50 # int | Maximum number of messages to return (optional) (default to 50)

    try:
        # List tenant messages
        api_response = api_instance.list_tenant_messages(cursor=cursor, limit=limit)
        print("The response of MessagesApi->list_tenant_messages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessagesApi->list_tenant_messages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cursor** | **str**| Opaque pagination cursor returned by a previous response | [optional] 
 **limit** | **int**| Maximum number of messages to return | [optional] [default to 50]

### Return type

[**TenantMessagesResponse**](TenantMessagesResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Tenant messages |  -  |
**401** | Missing or invalid credentials |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_email**
> SendEmailResponse send_email(send_email_request)

Send an email

Send a transactional email using the Dependal API.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import dependal
from dependal.models.send_email_request import SendEmailRequest
from dependal.models.send_email_response import SendEmailResponse
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
    api_instance = dependal.MessagesApi(api_client)
    send_email_request = {"from":"Dependal <noreply@dependal.com>","to":"developers@dependal.com","subject":"Dependal test send","html":"<p>Hello 👋</p><p>This is a transactional test email from Dependal.</p>"} # SendEmailRequest | 

    try:
        # Send an email
        api_response = api_instance.send_email(send_email_request)
        print("The response of MessagesApi->send_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessagesApi->send_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **send_email_request** | [**SendEmailRequest**](SendEmailRequest.md)|  | 

### Return type

[**SendEmailResponse**](SendEmailResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Accepted for delivery |  -  |
**400** | Request validation failed |  -  |
**401** | Missing or invalid credentials |  -  |
**403** | Sending blocked |  -  |
**409** | Conflict |  -  |
**413** | Payload too large |  -  |
**503** | Service unavailable |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

