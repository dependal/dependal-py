# ErrorBody


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | [**ErrorCode**](ErrorCode.md) |  | 
**message** | **str** |  | 
**fields** | **Dict[str, object]** | Optional field-level validation errors | [optional] 

## Example

```python
from dependal.models.error_body import ErrorBody

# TODO update the JSON string below
json = "{}"
# create an instance of ErrorBody from a JSON string
error_body_instance = ErrorBody.from_json(json)
# print the JSON string representation of the object
print(ErrorBody.to_json())

# convert the object into a dict
error_body_dict = error_body_instance.to_dict()
# create an instance of ErrorBody from a dict
error_body_from_dict = ErrorBody.from_dict(error_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


