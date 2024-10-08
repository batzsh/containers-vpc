# AWS Containers Architecture - VPC

![arch](/docs/diagram.png)

## Requirements

No requirements.

## Providers

| Name                                             | Version |
| ------------------------------------------------ | ------- |
| <a name="provider_aws"></a> [aws](#provider_aws) | 5.62.0  |

## Modules

No modules.

## Resources

| Name                                                                                                                                          | Type     |
| --------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| [aws_eip.vpc_eip_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip)                                         | resource |
| [aws_eip.vpc_eip_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip)                                         | resource |
| [aws_eip.vpc_eip_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip)                                         | resource |
| [aws_internet_gateway.gw](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway)                       | resource |
| [aws_nat_gateway.nat_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway)                             | resource |
| [aws_nat_gateway.nat_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway)                             | resource |
| [aws_nat_gateway.nat_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway)                             | resource |
| [aws_route.private_access_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route)                              | resource |
| [aws_route.private_access_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route)                              | resource |
| [aws_route.private_access_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route)                              | resource |
| [aws_route.public_access](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route)                                  | resource |
| [aws_route_table.private_internet_access_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table)         | resource |
| [aws_route_table.private_internet_access_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table)         | resource |
| [aws_route_table.private_internet_access_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table)         | resource |
| [aws_route_table.public_internet_access](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table)             | resource |
| [aws_route_table_association.private_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.private_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.private_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.public_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association)  | resource |
| [aws_route_table_association.public_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association)  | resource |
| [aws_route_table_association.public_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association)  | resource |
| [aws_ssm_parameter.databases_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                   | resource |
| [aws_ssm_parameter.databases_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                   | resource |
| [aws_ssm_parameter.databases_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                   | resource |
| [aws_ssm_parameter.private_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                     | resource |
| [aws_ssm_parameter.private_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                     | resource |
| [aws_ssm_parameter.private_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                     | resource |
| [aws_ssm_parameter.public_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                      | resource |
| [aws_ssm_parameter.public_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                      | resource |
| [aws_ssm_parameter.public_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                      | resource |
| [aws_ssm_parameter.vpc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter)                            | resource |
| [aws_subnet.databases_subnet_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                          | resource |
| [aws_subnet.databases_subnet_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                          | resource |
| [aws_subnet.databases_subnet_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                          | resource |
| [aws_subnet.private_subnet_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                            | resource |
| [aws_subnet.private_subnet_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                            | resource |
| [aws_subnet.private_subnet_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                            | resource |
| [aws_subnet.public_subnet_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                             | resource |
| [aws_subnet.public_subnet_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                             | resource |
| [aws_subnet.public_subnet_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet)                             | resource |
| [aws_vpc.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc)                                               | resource |

## Inputs

| Name                                                                  | Description                                                          | Type     | Default                                        | Required |
| --------------------------------------------------------------------- | -------------------------------------------------------------------- | -------- | ---------------------------------------------- | :------: |
| <a name="input_project_name"></a> [project_name](#input_project_name) | Project name performs as a prefix at all resources from this project | `any`    | n/a                                            |   yes    |
| <a name="input_region"></a> [region](#input_region)                   | n/a                                                                  | `string` | `"AWS Region where resources will be created"` |    no    |

## Outputs

| Name                                                                                                     | Description                                                                                                                                                                                     |
| -------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <a name="output_ssm_subnet_databases_1a"></a> [ssm_subnet_databases_1a](#output_ssm_subnet_databases_1a) | Databases subnet ID at availability zone 1a. This ID is retrieved from AWS Systems Manager Parameter Store and used for provisioning database instances in this specific zone.                  |
| <a name="output_ssm_subnet_databases_1b"></a> [ssm_subnet_databases_1b](#output_ssm_subnet_databases_1b) | Databases subnet ID at availability zone 1b. Obtained from AWS Systems Manager Parameter Store, it is essential for the allocation of database instances that need to be isolated in this zone. |
| <a name="output_ssm_subnet_databases_1c"></a> [ssm_subnet_databases_1c](#output_ssm_subnet_databases_1c) | Databases subnet ID at availability zone 1c, sourced from AWS Systems Manager Parameter Store. Used in provisioning database instances that require isolation in this zone.                     |
| <a name="output_ssm_subnet_private_1a"></a> [ssm_subnet_private_1a](#output_ssm_subnet_private_1a)       | Private subnet ID at availability zone 1a. Value stored in AWS Systems Manager Parameter Store, used to provision resources in a specific private subnet.                                       |
| <a name="output_ssm_subnet_private_1b"></a> [ssm_subnet_private_1b](#output_ssm_subnet_private_1b)       | Private subnet ID at availability zone 1b. Stored in AWS Systems Manager Parameter Store, used for resource allocation that requires isolation within this availability zone.                   |
| <a name="output_ssm_subnet_private_1c"></a> [ssm_subnet_private_1c](#output_ssm_subnet_private_1c)       | Private subnet ID at availability zone 1c. Stored in AWS Systems Manager Parameter Store, crucial for the creation of resources that need to be isolated in this specific zone.                 |
| <a name="output_ssm_subnet_public_1a"></a> [ssm_subnet_public_1a](#output_ssm_subnet_public_1a)          | Public subnet ID at availability zone 1a. This ID, sourced from AWS Systems Manager Parameter Store, is used to provision publicly accessible resources in this zone.                           |
| <a name="output_ssm_subnet_public_1b"></a> [ssm_subnet_public_1b](#output_ssm_subnet_public_1b)          | Public subnet ID at availability zone 1b. Available via AWS Systems Manager Parameter Store, it enables the deployment of resources with public access in this specific zone.                   |
| <a name="output_ssm_subnet_public_1c"></a> [ssm_subnet_public_1c](#output_ssm_subnet_public_1c)          | Public subnet ID at availability zone 1c, stored in AWS Systems Manager Parameter Store. Used to configure resources that require public access in this zone.                                   |
| <a name="output_ssm_vpc_id"></a> [ssm_vpc_id](#output_ssm_vpc_id)                                        | VPC ID stored at AWS Systems Manager Parameter Store. This ID is used to identify the VPC where the resources will be provisioned.                                                              |
