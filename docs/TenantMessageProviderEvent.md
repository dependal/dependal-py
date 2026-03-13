# TenantMessageProviderEvent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_at_iso** | **datetime** |  | 
**recipient** | **str** |  | 
**provider_message_id** | **str** |  | 
**message_id** | **UUID** |  | 
**meta** | [**TenantMessageProviderMeta**](TenantMessageProviderMeta.md) |  | 
**tenant_id** | **UUID** |  | 
**event_at** | **int** | Unix timestamp in seconds | 
**provider** | [**ProviderEnum**](ProviderEnum.md) |  | 
**event_type** | [**MessageStatusEnum**](MessageStatusEnum.md) |  | 
**event_group** | [**EventGroupEnum**](EventGroupEnum.md) |  | 

## Example

```python
from dependal.models.tenant_message_provider_event import TenantMessageProviderEvent

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageProviderEvent from a JSON string
tenant_message_provider_event_instance = TenantMessageProviderEvent.from_json(json)
# print the JSON string representation of the object
print(TenantMessageProviderEvent.to_json())

# convert the object into a dict
tenant_message_provider_event_dict = tenant_message_provider_event_instance.to_dict()
# create an instance of TenantMessageProviderEvent from a dict
tenant_message_provider_event_from_dict = TenantMessageProviderEvent.from_dict(tenant_message_provider_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


