# TenantMessageEvent


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
**event_type** | **str** |  | 
**event_group** | [**EventGroupEnum**](EventGroupEnum.md) |  | 
**stage** | [**StageEnum**](StageEnum.md) |  | 
**detail** | **Dict[str, object]** |  | 
**caller_type** | [**CallerTypeEnum**](CallerTypeEnum.md) |  | 
**status** | [**MessageStatusEnum**](MessageStatusEnum.md) |  | 
**source** | [**SourceEnum**](SourceEnum.md) |  | 
**created_at_iso** | **datetime** |  | 
**reason** | **str** |  | 
**request_id** | **UUID** |  | 
**tag** | **str** |  | 

## Example

```python
from dependal.models.tenant_message_event import TenantMessageEvent

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageEvent from a JSON string
tenant_message_event_instance = TenantMessageEvent.from_json(json)
# print the JSON string representation of the object
print(TenantMessageEvent.to_json())

# convert the object into a dict
tenant_message_event_dict = tenant_message_event_instance.to_dict()
# create an instance of TenantMessageEvent from a dict
tenant_message_event_from_dict = TenantMessageEvent.from_dict(tenant_message_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


