# TenantMessageInternalEvent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**stage** | [**StageEnum**](StageEnum.md) |  | 
**detail** | **Dict[str, object]** |  | 
**tenant_id** | **UUID** |  | 
**caller_type** | [**CallerTypeEnum**](CallerTypeEnum.md) |  | 
**status** | [**MessageStatusEnum**](MessageStatusEnum.md) |  | 
**source** | [**SourceEnum**](SourceEnum.md) |  | 
**created_at_iso** | **datetime** |  | 
**reason** | **str** |  | 
**request_id** | **UUID** |  | 
**event_at_iso** | **datetime** |  | 
**event_type** | **str** |  | 
**tag** | **str** |  | 
**event_group** | [**EventGroupEnum**](EventGroupEnum.md) |  | 

## Example

```python
from openapi_client.models.tenant_message_internal_event import TenantMessageInternalEvent

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageInternalEvent from a JSON string
tenant_message_internal_event_instance = TenantMessageInternalEvent.from_json(json)
# print the JSON string representation of the object
print(TenantMessageInternalEvent.to_json())

# convert the object into a dict
tenant_message_internal_event_dict = tenant_message_internal_event_instance.to_dict()
# create an instance of TenantMessageInternalEvent from a dict
tenant_message_internal_event_from_dict = TenantMessageInternalEvent.from_dict(tenant_message_internal_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


