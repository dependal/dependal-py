# TenantMessageEventHeader


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**value** | **str** |  | 

## Example

```python
from openapi_client.models.tenant_message_event_header import TenantMessageEventHeader

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageEventHeader from a JSON string
tenant_message_event_header_instance = TenantMessageEventHeader.from_json(json)
# print the JSON string representation of the object
print(TenantMessageEventHeader.to_json())

# convert the object into a dict
tenant_message_event_header_dict = tenant_message_event_header_instance.to_dict()
# create an instance of TenantMessageEventHeader from a dict
tenant_message_event_header_from_dict = TenantMessageEventHeader.from_dict(tenant_message_event_header_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


