# Service Bus Namespace Migration Configuration `[Microsoft.ServiceBus/namespaces/migrationConfigurations]`

This module deploys a Service Bus Namespace Migration Configuration.

## Navigation

- [Resource Types](#Resource-Types)
- [Parameters](#Parameters)
- [Outputs](#Outputs)
- [Cross-referenced modules](#Cross-referenced-modules)

## Resource Types

| Resource Type | API Version |
| :-- | :-- |
| `Microsoft.ServiceBus/namespaces/migrationConfigurations` | [2022-10-01-preview](https://learn.microsoft.com/en-us/azure/templates/Microsoft.ServiceBus/2022-10-01-preview/namespaces/migrationConfigurations) |

## Parameters

**Required parameters**

| Parameter Name | Type | Description |
| :-- | :-- | :-- |
| `postMigrationName` | string | Name to access Standard Namespace after migration. |
| `targetNamespaceResourceId` | string | Existing premium Namespace resource ID which has no entities, will be used for migration. |

**Conditional parameters**

| Parameter Name | Type | Description |
| :-- | :-- | :-- |
| `namespaceName` | string | The name of the parent Service Bus Namespace for the Service Bus Queue. Required if the template is used in a standalone deployment. |

**Optional parameters**

| Parameter Name | Type | Default Value | Description |
| :-- | :-- | :-- | :-- |
| `enableDefaultTelemetry` | bool | `True` | Enable telemetry via a Globally Unique Identifier (GUID). |


## Outputs

| Output Name | Type | Description |
| :-- | :-- | :-- |
| `name` | string | The name of the migration configuration. |
| `resourceGroupName` | string | The name of the Resource Group the migration configuration was created in. |
| `resourceId` | string | The Resource ID of the migration configuration. |

## Cross-referenced modules

_None_
