# TenantMessageMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delivery** | [**TenantMessageMetaDelivery**](TenantMessageMetaDelivery.md) |  | 

## Example

```python
from dependal.models.tenant_message_meta import TenantMessageMeta

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageMeta from a JSON string
tenant_message_meta_instance = TenantMessageMeta.from_json(json)
# print the JSON string representation of the object
print(TenantMessageMeta.to_json())

# convert the object into a dict
tenant_message_meta_dict = tenant_message_meta_instance.to_dict()
# create an instance of TenantMessageMeta from a dict
tenant_message_meta_from_dict = TenantMessageMeta.from_dict(tenant_message_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


