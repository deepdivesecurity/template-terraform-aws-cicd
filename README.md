# Template - Terraform AWS CI/CD Pipeline

![Terraform CI/CD](https://github.com/deepdivesecurity/terraform-aws-org/actions/workflows/terraform-cicd.yml/badge.svg)

## Description
This repo contains the template structure and CI/CD pipeline for deploying to AWS. It expects that the user has already configured an AWS S3 bucket for state file management.
If you haven't done so, you can find a sample at the following GitHub repo (Note that unlike the following link, this repo expects the use of S3 state locking rather than the deprecated DynamoDB state locking mechanism): https://github.com/aws-samples/manage-terraform-statefiles-in-aws-pipeline/tree/main

## GitHub Repo Secrets
| Name | Description |
|------|-------------|
| AWS_ROLE_ARN | 
| AWS_REGION | Your AWS region (e.g. "ca-central-1") |
| TF_BACKEND_BUCKET | Your Terraform backend S3 bucket for storing your Terraform state file in (e.g. "mybucket") |
| TF_BACKEND_KEY | The path to your Terraform state object (e.g. "path/to/my/key") |

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.12.0 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 6.3.0 |

## Providers

No providers.

## Modules

No modules.

## Resources

No resources.

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | n/a | `string` | `"ca-central-1"` | no |

## Outputs

No outputs.
<!-- END_TF_DOCS -->