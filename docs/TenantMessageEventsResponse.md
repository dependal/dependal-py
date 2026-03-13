# TenantMessageEventsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TenantMessageEventsPage**](TenantMessageEventsPage.md) |  | 

## Example

```python
from openapi_client.models.tenant_message_events_response import TenantMessageEventsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageEventsResponse from a JSON string
tenant_message_events_response_instance = TenantMessageEventsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantMessageEventsResponse.to_json())

# convert the object into a dict
tenant_message_events_response_dict = tenant_message_events_response_instance.to_dict()
# create an instance of TenantMessageEventsResponse from a dict
tenant_message_events_response_from_dict = TenantMessageEventsResponse.from_dict(tenant_message_events_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


