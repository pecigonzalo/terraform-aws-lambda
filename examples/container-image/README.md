# AWS Lambda launched from Docker Container Image example

Configuration in this directory creates AWS Lambda Function deployed with a Container Image.

## Usage

To run this example you need to execute:

```bash
$ terraform init
$ terraform plan
$ terraform apply
```

Note that this example may create resources which cost money. Run `terraform destroy` when you don't need these resources.

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| terraform | >= 0.13.0 |
| aws | >= 3.19 |
| docker | >= 2.8.0 |
| random | >= 2 |

## Providers

| Name | Version |
|------|---------|
| aws | >= 3.19 |
| docker | >= 2.8.0 |
| random | >= 2 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| lambda_function_from_container_image | ../../ |  |

## Resources

| Name |
|------|
| [aws_caller_identity](https://registry.terraform.io/providers/hashicorp/aws/3.19/docs/data-sources/caller_identity) |
| [aws_ecr_authorization_token](https://registry.terraform.io/providers/hashicorp/aws/3.19/docs/data-sources/ecr_authorization_token) |
| [aws_ecr_repository](https://registry.terraform.io/providers/hashicorp/aws/3.19/docs/resources/ecr_repository) |
| [aws_region](https://registry.terraform.io/providers/hashicorp/aws/3.19/docs/data-sources/region) |
| [docker_registry_image](https://registry.terraform.io/providers/kreuzwerker/docker/2.8.0/docs/resources/registry_image) |
| [random_pet](https://registry.terraform.io/providers/hashicorp/random/2/docs/resources/pet) |

## Inputs

No input.

## Outputs

| Name | Description |
|------|-------------|
| lambda\_cloudwatch\_log\_group\_arn | The ARN of the Cloudwatch Log Group |
| lambda\_role\_arn | The ARN of the IAM role created for the Lambda Function |
| lambda\_role\_name | The name of the IAM role created for the Lambda Function |
| this\_lambda\_function\_arn | The ARN of the Lambda Function |
| this\_lambda\_function\_invoke\_arn | The Invoke ARN of the Lambda Function |
| this\_lambda\_function\_kms\_key\_arn | The ARN for the KMS encryption key of Lambda Function |
| this\_lambda\_function\_last\_modified | The date Lambda Function resource was last modified |
| this\_lambda\_function\_name | The name of the Lambda Function |
| this\_lambda\_function\_qualified\_arn | The ARN identifying your Lambda Function Version |
| this\_lambda\_function\_source\_code\_hash | Base64-encoded representation of raw SHA-256 sum of the zip file |
| this\_lambda\_function\_source\_code\_size | The size in bytes of the function .zip file |
| this\_lambda\_function\_version | Latest published version of Lambda Function |
| this\_lambda\_layer\_arn | The ARN of the Lambda Layer with version |
| this\_lambda\_layer\_created\_date | The date Lambda Layer resource was created |
| this\_lambda\_layer\_layer\_arn | The ARN of the Lambda Layer without version |
| this\_lambda\_layer\_source\_code\_size | The size in bytes of the Lambda Layer .zip file |
| this\_lambda\_layer\_version | The Lambda Layer version |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
