# TenantDomainDetailResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TenantDomainDetail**](TenantDomainDetail.md) |  | 

## Example

```python
from openapi_client.models.tenant_domain_detail_response import TenantDomainDetailResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainDetailResponse from a JSON string
tenant_domain_detail_response_instance = TenantDomainDetailResponse.from_json(json)
# print the JSON string representation of the object
print(TenantDomainDetailResponse.to_json())

# convert the object into a dict
tenant_domain_detail_response_dict = tenant_domain_detail_response_instance.to_dict()
# create an instance of TenantDomainDetailResponse from a dict
tenant_domain_detail_response_from_dict = TenantDomainDetailResponse.from_dict(tenant_domain_detail_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


