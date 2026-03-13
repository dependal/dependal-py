# TenantMessageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TenantMessage**](TenantMessage.md) |  | 

## Example

```python
from dependal.models.tenant_message_response import TenantMessageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageResponse from a JSON string
tenant_message_response_instance = TenantMessageResponse.from_json(json)
# print the JSON string representation of the object
print(TenantMessageResponse.to_json())

# convert the object into a dict
tenant_message_response_dict = tenant_message_response_instance.to_dict()
# create an instance of TenantMessageResponse from a dict
tenant_message_response_from_dict = TenantMessageResponse.from_dict(tenant_message_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


