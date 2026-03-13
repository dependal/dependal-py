# TenantDomainCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** |  | 
**status** | [**DomainStatusEnum**](DomainStatusEnum.md) |  | 

## Example

```python
from dependal.models.tenant_domain_create import TenantDomainCreate

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainCreate from a JSON string
tenant_domain_create_instance = TenantDomainCreate.from_json(json)
# print the JSON string representation of the object
print(TenantDomainCreate.to_json())

# convert the object into a dict
tenant_domain_create_dict = tenant_domain_create_instance.to_dict()
# create an instance of TenantDomainCreate from a dict
tenant_domain_create_from_dict = TenantDomainCreate.from_dict(tenant_domain_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


