# TenantMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **UUID** |  | 
**request_id** | **UUID** |  | 
**status** | [**MessageStatusEnum**](MessageStatusEnum.md) |  | 
**reason** | **str** |  | 
**created_at** | **int** | Unix timestamp in seconds | 
**updated_at** | **int** | Unix timestamp in seconds | 
**last_event_at** | **int** | Unix timestamp in seconds of the latest known event | 
**created_at_iso** | **datetime** |  | 
**updated_at_iso** | **datetime** |  | 
**last_event_at_iso** | **datetime** |  | 
**to** | **str** |  | 
**var_from** | **str** |  | 
**subject** | **str** |  | 
**source_ip** | **str** |  | 
**stage** | [**StageEnum**](StageEnum.md) |  | 
**tag** | **str** |  | 
**key_id** | **str** |  | 
**caller_type** | [**CallerTypeEnum**](CallerTypeEnum.md) |  | 
**last_source** | [**SourceEnum**](SourceEnum.md) |  | 
**last_event_type** | [**MessageStatusEnum**](MessageStatusEnum.md) |  | 
**ses_message_id** | **str** |  | 
**idempotency_key** | **str** |  | 
**metadata** | **Dict[str, object]** |  | 
**meta** | [**TenantMessageMeta**](TenantMessageMeta.md) |  | 

## Example

```python
from dependal.models.tenant_message import TenantMessage

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessage from a JSON string
tenant_message_instance = TenantMessage.from_json(json)
# print the JSON string representation of the object
print(TenantMessage.to_json())

# convert the object into a dict
tenant_message_dict = tenant_message_instance.to_dict()
# create an instance of TenantMessage from a dict
tenant_message_from_dict = TenantMessage.from_dict(tenant_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


