## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| azurerm | n/a |
| helm | n/a |
| kubernetes-alpha | n/a |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| address\_prefixes | (Required) The address prefixes to use for the subnet. | `list(string)` | n/a | yes |
| address\_space | (Required) The list of the ip address ranges for the vnet | `list(any)` | n/a | yes |
| environment | Development environment for resource; prod, non-prod, shared-services | `string` | n/a | yes |
| key\_vault\_name | Name of key vault to use with CSI driver | `string` | n/a | yes |
| kubernetes\_version | Version of Kubernetes specified when creating the AKS managed cluster. If not specified, the latest recommended version will be used at provisioning time (but won't auto-upgrade). | `string` | `null` | no |
| name\_prefix | A short pre-defined text to identify the resource type | `string` | `"aks"` | no |
| random\_string\_result | The generated random string. | `string` | n/a | yes |
| region | Geographic Region resource will be deployed into | `string` | n/a | yes |
| resource\_group\_name | (Required) The Name of this Resource Group. | `string` | n/a | yes |
| tags | A map of tags to add to all resources | `map(any)` | `{}` | no |
| vm\_size | (Required) The size of the Virtual Machine, such as Standard\_DS2\_v2. | `string` | `"Standard_DS2_v2"` | no |

## Outputs

| Name | Description |
|------|-------------|
| acr\_name | n/a |
| fqdn | n/a |
| id | n/a |
| kube\_config\_client\_certificate | n/a |
| kube\_config\_client\_key | n/a |
| kube\_config\_cluster\_ca\_certificate | n/a |
| kube\_config\_host | n/a |
| kube\_config\_password | n/a |
| kube\_config\_raw | n/a |
| kube\_config\_username | n/a |
| kubelet\_identity\_object\_id | n/a |
| name | n/a |
| node\_resource\_group | n/a |