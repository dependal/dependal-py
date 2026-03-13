# TenantMessageEventDelivery


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**smtp_response** | **str** |  | [optional] 
**processing_time_millis** | **int** |  | [optional] 
**reporting_mta** | **str** |  | [optional] 
**remote_mta_ip** | **str** |  | [optional] 
**recipients** | **List[str]** |  | [optional] 
**timestamp** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.tenant_message_event_delivery import TenantMessageEventDelivery

# TODO update the JSON string below
json = "{}"
# create an instance of TenantMessageEventDelivery from a JSON string
tenant_message_event_delivery_instance = TenantMessageEventDelivery.from_json(json)
# print the JSON string representation of the object
print(TenantMessageEventDelivery.to_json())

# convert the object into a dict
tenant_message_event_delivery_dict = tenant_message_event_delivery_instance.to_dict()
# create an instance of TenantMessageEventDelivery from a dict
tenant_message_event_delivery_from_dict = TenantMessageEventDelivery.from_dict(tenant_message_event_delivery_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


