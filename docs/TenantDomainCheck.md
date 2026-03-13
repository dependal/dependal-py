# TenantDomainCheck


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** |  | 
**status** | [**DomainStatusEnum**](DomainStatusEnum.md) |  | 
**ses** | [**TenantDomainSesStatus**](TenantDomainSesStatus.md) |  | 

## Example

```python
from openapi_client.models.tenant_domain_check import TenantDomainCheck

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainCheck from a JSON string
tenant_domain_check_instance = TenantDomainCheck.from_json(json)
# print the JSON string representation of the object
print(TenantDomainCheck.to_json())

# convert the object into a dict
tenant_domain_check_dict = tenant_domain_check_instance.to_dict()
# create an instance of TenantDomainCheck from a dict
tenant_domain_check_from_dict = TenantDomainCheck.from_dict(tenant_domain_check_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


