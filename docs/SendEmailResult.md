# SendEmailResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **UUID** |  | 
**status** | [**MessageStatusEnum**](MessageStatusEnum.md) |  | 

## Example

```python
from dependal.models.send_email_result import SendEmailResult

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailResult from a JSON string
send_email_result_instance = SendEmailResult.from_json(json)
# print the JSON string representation of the object
print(SendEmailResult.to_json())

# convert the object into a dict
send_email_result_dict = send_email_result_instance.to_dict()
# create an instance of SendEmailResult from a dict
send_email_result_from_dict = SendEmailResult.from_dict(send_email_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


