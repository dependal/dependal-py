# TenantDomainSesStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**verification_status** | [**SesVerificationStatusEnum**](SesVerificationStatusEnum.md) |  | 
**dkim_status** | [**SesVerificationStatusEnum**](SesVerificationStatusEnum.md) |  | 

## Example

```python
from openapi_client.models.tenant_domain_ses_status import TenantDomainSesStatus

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainSesStatus from a JSON string
tenant_domain_ses_status_instance = TenantDomainSesStatus.from_json(json)
# print the JSON string representation of the object
print(TenantDomainSesStatus.to_json())

# convert the object into a dict
tenant_domain_ses_status_dict = tenant_domain_ses_status_instance.to_dict()
# create an instance of TenantDomainSesStatus from a dict
tenant_domain_ses_status_from_dict = TenantDomainSesStatus.from_dict(tenant_domain_ses_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


