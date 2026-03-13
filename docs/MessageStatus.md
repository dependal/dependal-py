# MessageStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **UUID** |  | 
**status** | [**MessageStatusEnum**](MessageStatusEnum.md) |  | 
**reason** | **str** | Optional reason for failure, bounce, complaint, or rejection | 
**created_at** | **int** | Unix timestamp in seconds | 
**updated_at** | **int** | Unix timestamp in seconds | 
**to** | **str** |  | 
**var_from** | **str** |  | 
**subject** | **str** |  | 
**sending_message_id** | **str** | Provider message identifier | 

## Example

```python
from dependal.models.message_status import MessageStatus

# TODO update the JSON string below
json = "{}"
# create an instance of MessageStatus from a JSON string
message_status_instance = MessageStatus.from_json(json)
# print the JSON string representation of the object
print(MessageStatus.to_json())

# convert the object into a dict
message_status_dict = message_status_instance.to_dict()
# create an instance of MessageStatus from a dict
message_status_from_dict = MessageStatus.from_dict(message_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


