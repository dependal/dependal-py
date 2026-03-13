# TenantMessageProviderMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mail** | [**TenantMessageEventMail**](TenantMessageEventMail.md) |  | [optional] 
**send** | **Dict[str, object]** |  | [optional] 
**delivery** | [**TenantMessageEventDelivery**](TenantMessageEventDelivery.md) |  | [optional] 
**provider_event_type** | [**ProviderEventTypeEnum**](ProviderEventTypeEnum.md) |  | [optional] 

## Example

```python
from dependal.models.tenant_message_provider_meta import TenantMessageProviderMeta

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageProviderMeta from a JSON string
tenant_message_provider_meta_instance = TenantMessageProviderMeta.from_json(json)
# print the JSON string representation of the object
print(TenantMessageProviderMeta.to_json())

# convert the object into a dict
tenant_message_provider_meta_dict = tenant_message_provider_meta_instance.to_dict()
# create an instance of TenantMessageProviderMeta from a dict
tenant_message_provider_meta_from_dict = TenantMessageProviderMeta.from_dict(tenant_message_provider_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


