# TenantPoliciesAcceptResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TenantPoliciesAccept**](TenantPoliciesAccept.md) |  | 

## Example

```python
from dependal.models.tenant_policies_accept_response import TenantPoliciesAcceptResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantPoliciesAcceptResponse from a JSON string
tenant_policies_accept_response_instance = TenantPoliciesAcceptResponse.from_json(json)
# print the JSON string representation of the object
print(TenantPoliciesAcceptResponse.to_json())

# convert the object into a dict
tenant_policies_accept_response_dict = tenant_policies_accept_response_instance.to_dict()
# create an instance of TenantPoliciesAcceptResponse from a dict
tenant_policies_accept_response_from_dict = TenantPoliciesAcceptResponse.from_dict(tenant_policies_accept_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


