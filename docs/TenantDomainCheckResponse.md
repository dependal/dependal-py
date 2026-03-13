# TenantDomainCheckResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TenantDomainCheck**](TenantDomainCheck.md) |  | 

## Example

```python
from dependal.models.tenant_domain_check_response import TenantDomainCheckResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainCheckResponse from a JSON string
tenant_domain_check_response_instance = TenantDomainCheckResponse.from_json(json)
# print the JSON string representation of the object
print(TenantDomainCheckResponse.to_json())

# convert the object into a dict
tenant_domain_check_response_dict = tenant_domain_check_response_instance.to_dict()
# create an instance of TenantDomainCheckResponse from a dict
tenant_domain_check_response_from_dict = TenantDomainCheckResponse.from_dict(tenant_domain_check_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


