# TenantDomainDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** |  | 
**mail_from_domain** | **str** |  | 
**status** | [**DomainStatusEnum**](DomainStatusEnum.md) |  | 
**ses** | [**TenantDomainSesStatus**](TenantDomainSesStatus.md) |  | 
**records** | [**List[TenantDomainRecord]**](TenantDomainRecord.md) |  | 

## Example

```python
from openapi_client.models.tenant_domain_detail import TenantDomainDetail

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainDetail from a JSON string
tenant_domain_detail_instance = TenantDomainDetail.from_json(json)
# print the JSON string representation of the object
print(TenantDomainDetail.to_json())

# convert the object into a dict
tenant_domain_detail_dict = tenant_domain_detail_instance.to_dict()
# create an instance of TenantDomainDetail from a dict
tenant_domain_detail_from_dict = TenantDomainDetail.from_dict(tenant_domain_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


