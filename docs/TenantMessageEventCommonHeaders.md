# TenantMessageEventCommonHeaders


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** |  | 
**var_from** | **List[str]** |  | 
**to** | **List[str]** |  | 
**subject** | **str** |  | 

## Example

```python
from dependal.models.tenant_message_event_common_headers import TenantMessageEventCommonHeaders

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageEventCommonHeaders from a JSON string
tenant_message_event_common_headers_instance = TenantMessageEventCommonHeaders.from_json(json)
# print the JSON string representation of the object
print(TenantMessageEventCommonHeaders.to_json())

# convert the object into a dict
tenant_message_event_common_headers_dict = tenant_message_event_common_headers_instance.to_dict()
# create an instance of TenantMessageEventCommonHeaders from a dict
tenant_message_event_common_headers_from_dict = TenantMessageEventCommonHeaders.from_dict(tenant_message_event_common_headers_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


