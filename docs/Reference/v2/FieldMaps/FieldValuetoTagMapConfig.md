## FieldMaps: FieldValuetoTagMapConfig

>**_This documentation is for a preview version of the Azure DevOps Migration Tools._ If you are not using the preview version then please head over to the main [documentation](https://nkdagility.github.io/azure-devops-migration-tools).**

[Overview](../../../index.md) > [Reference](../../index.md) > [API v2](../index.md) > [FieldMaps](index.md)> **FieldValuetoTagMapConfig**

Need to create a Tag based on a field value? Just create a regex match and choose how to populate the target.

### Options

| Parameter name         | Type    | Description                              | Default Value                            |
|------------------------|---------|------------------------------------------|------------------------------------------|
| formatExpression | String | missng XML code comments | missng XML code comments |
| pattern | String | missng XML code comments | missng XML code comments |
| sourceField | String | missng XML code comments | missng XML code comments |
| WorkItemTypeName | String | missng XML code comments | missng XML code comments |


### Example JSON

```JSON
{
  "$type": "FieldValuetoTagMapConfig",
  "WorkItemTypeName": "*",
  "sourceField": "System.Status",
  "pattern": "(Active|Resolved)",
  "formatExpression": "Status: {0}"
}
```