# TenantDomainCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** | Domain to register for sending | 

## Example

```python
from dependal.models.tenant_domain_create_request import TenantDomainCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainCreateRequest from a JSON string
tenant_domain_create_request_instance = TenantDomainCreateRequest.from_json(json)
# print the JSON string representation of the object
print(TenantDomainCreateRequest.to_json())

# convert the object into a dict
tenant_domain_create_request_dict = tenant_domain_create_request_instance.to_dict()
# create an instance of TenantDomainCreateRequest from a dict
tenant_domain_create_request_from_dict = TenantDomainCreateRequest.from_dict(tenant_domain_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


