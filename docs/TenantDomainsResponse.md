# TenantDomainsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[TenantDomain]**](TenantDomain.md) |  | 

## Example

```python
from openapi_client.models.tenant_domains_response import TenantDomainsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainsResponse from a JSON string
tenant_domains_response_instance = TenantDomainsResponse.from_json(json)
# print the JSON string representation of the object
print(TenantDomainsResponse.to_json())

# convert the object into a dict
tenant_domains_response_dict = tenant_domains_response_instance.to_dict()
# create an instance of TenantDomainsResponse from a dict
tenant_domains_response_from_dict = TenantDomainsResponse.from_dict(tenant_domains_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


