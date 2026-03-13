# TenantDomain


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** |  | 
**status** | [**DomainStatusEnum**](DomainStatusEnum.md) |  | 
**created_at** | **int** | Unix timestamp in seconds | 
**verified_at** | **int** | Unix timestamp in seconds when the domain was verified | 
**updated_at** | **datetime** |  | 

## Example

```python
from dependal.models.tenant_domain import TenantDomain

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomain from a JSON string
tenant_domain_instance = TenantDomain.from_json(json)
# print the JSON string representation of the object
print(TenantDomain.to_json())

# convert the object into a dict
tenant_domain_dict = tenant_domain_instance.to_dict()
# create an instance of TenantDomain from a dict
tenant_domain_from_dict = TenantDomain.from_dict(tenant_domain_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


