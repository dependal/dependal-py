# TenantMessagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TenantMessagesPage**](TenantMessagesPage.md) |  | 

## Example

```python
from dependal.models.tenant_messages_response import TenantMessagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessagesResponse from a JSON string
tenant_messages_response_instance = TenantMessagesResponse.from_json(json)
# print the JSON string representation of the object
print(TenantMessagesResponse.to_json())

# convert the object into a dict
tenant_messages_response_dict = tenant_messages_response_instance.to_dict()
# create an instance of TenantMessagesResponse from a dict
tenant_messages_response_from_dict = TenantMessagesResponse.from_dict(tenant_messages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


