# TenantDomainRecord


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | [**DnsRecordTypeEnum**](DnsRecordTypeEnum.md) |  | 
**name** | **str** |  | 
**value** | **str** |  | 

## Example

```python
from openapi_client.models.tenant_domain_record import TenantDomainRecord

# TODO update the JSON string below
json = "{}"
# create an instance of TenantDomainRecord from a JSON string
tenant_domain_record_instance = TenantDomainRecord.from_json(json)
# print the JSON string representation of the object
print(TenantDomainRecord.to_json())

# convert the object into a dict
tenant_domain_record_dict = tenant_domain_record_instance.to_dict()
# create an instance of TenantDomainRecord from a dict
tenant_domain_record_from_dict = TenantDomainRecord.from_dict(tenant_domain_record_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


