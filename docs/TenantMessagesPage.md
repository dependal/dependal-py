# TenantMessagesPage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[TenantMessage]**](TenantMessage.md) |  | 
**cursor** | **str** | Opaque pagination cursor for the next page | 

## Example

```python
from dependal.models.tenant_messages_page import TenantMessagesPage

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessagesPage from a JSON string
tenant_messages_page_instance = TenantMessagesPage.from_json(json)
# print the JSON string representation of the object
print(TenantMessagesPage.to_json())

# convert the object into a dict
tenant_messages_page_dict = tenant_messages_page_instance.to_dict()
# create an instance of TenantMessagesPage from a dict
tenant_messages_page_from_dict = TenantMessagesPage.from_dict(tenant_messages_page_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


