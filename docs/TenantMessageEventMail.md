# TenantMessageEventMail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source_arn** | **str** |  | [optional] 
**headers** | [**List[TenantMessageEventHeader]**](TenantMessageEventHeader.md) |  | [optional] 
**sending_account_id** | **str** |  | [optional] 
**destination** | **List[str]** |  | [optional] 
**headers_truncated** | **bool** |  | [optional] 
**message_id** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**timestamp** | **datetime** |  | [optional] 
**common_headers** | [**TenantMessageEventCommonHeaders**](TenantMessageEventCommonHeaders.md) |  | [optional] 
**tags** | **Dict[str, List[str]]** |  | [optional] 

## Example

```python
from openapi_client.models.tenant_message_event_mail import TenantMessageEventMail

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageEventMail from a JSON string
tenant_message_event_mail_instance = TenantMessageEventMail.from_json(json)
# print the JSON string representation of the object
print(TenantMessageEventMail.to_json())

# convert the object into a dict
tenant_message_event_mail_dict = tenant_message_event_mail_instance.to_dict()
# create an instance of TenantMessageEventMail from a dict
tenant_message_event_mail_from_dict = TenantMessageEventMail.from_dict(tenant_message_event_mail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


