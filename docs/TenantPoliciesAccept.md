# TenantPoliciesAccept


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**accepted_version** | **str** | Policy version the tenant just accepted | 
**required_policy_version** | **str** | Current policy version required by the platform | 

## Example

```python
from dependal.models.tenant_policies_accept import TenantPoliciesAccept

# TODO update the JSON string below
json = "{}"
# create an instance of TenantPoliciesAccept from a JSON string
tenant_policies_accept_instance = TenantPoliciesAccept.from_json(json)
# print the JSON string representation of the object
print(TenantPoliciesAccept.to_json())

# convert the object into a dict
tenant_policies_accept_dict = tenant_policies_accept_instance.to_dict()
# create an instance of TenantPoliciesAccept from a dict
tenant_policies_accept_from_dict = TenantPoliciesAccept.from_dict(tenant_policies_accept_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


