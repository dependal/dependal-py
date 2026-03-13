# TenantMessageEventsPage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[TenantMessageEvent]**](TenantMessageEvent.md) |  | 
**cursor** | **str** | Opaque pagination cursor for the next page | 

## Example

```python
from openapi_client.models.tenant_message_events_page import TenantMessageEventsPage

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageEventsPage from a JSON string
tenant_message_events_page_instance = TenantMessageEventsPage.from_json(json)
# print the JSON string representation of the object
print(TenantMessageEventsPage.to_json())

# convert the object into a dict
tenant_message_events_page_dict = tenant_message_events_page_instance.to_dict()
# create an instance of TenantMessageEventsPage from a dict
tenant_message_events_page_from_dict = TenantMessageEventsPage.from_dict(tenant_message_events_page_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


