# SendEmailRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_from** | **str** | Sender in RFC 5322 mailbox format | 
**to** | **str** | Recipient email address | 
**subject** | **str** |  | 
**text** | **str** |  | [optional] 
**html** | **str** |  | [optional] 
**tags** | **Dict[str, str]** | Optional message tags | [optional] 

## Example

```python
from dependal.models.send_email_request import SendEmailRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailRequest from a JSON string
send_email_request_instance = SendEmailRequest.from_json(json)
# print the JSON string representation of the object
print(SendEmailRequest.to_json())

# convert the object into a dict
send_email_request_dict = send_email_request_instance.to_dict()
# create an instance of SendEmailRequest from a dict
send_email_request_from_dict = SendEmailRequest.from_dict(send_email_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


