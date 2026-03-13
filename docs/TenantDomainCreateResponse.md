# TenantDomainCreateResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TenantDomainCreate**](TenantDomainCreate.md) |  | 

## Example

```python
from openapi_client.models.tenant_domain_create_response import TenantDomainCreateResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainCreateResponse from a JSON string
tenant_domain_create_response_instance = TenantDomainCreateResponse.from_json(json)
# print the JSON string representation of the object
print(TenantDomainCreateResponse.to_json())

# convert the object into a dict
tenant_domain_create_response_dict = tenant_domain_create_response_instance.to_dict()
# create an instance of TenantDomainCreateResponse from a dict
tenant_domain_create_response_from_dict = TenantDomainCreateResponse.from_dict(tenant_domain_create_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


