---
api_key_in:
- header
api_specs:
- filename: aws-cost-explorer-api-openapi.yml
  format: yaml
  label: AWS Cost Explorer API
  slug: aws-cost-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/aws-cost-explorer-api-openapi.yml
- filename: aws-budgets-api-openapi.yml
  format: yaml
  label: AWS Budgets API
  slug: aws-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/aws-budgets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Billing And Cost Management Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Billing And Cost Management secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Billing And Cost Management
provider_slug: amazon-billing-and-cost-management
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_iam
  parameter: Authorization
  sources:
  - openapi/aws-budgets-api-openapi.yml
  - openapi/aws-cost-explorer-api-openapi.yml
  type: apiKey
slug: amazon-billing-and-cost-management-authentication
source_filename: amazon-billing-and-cost-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-budgets-api-openapi.yml, openapi/aws-cost-explorer-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_iam\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/aws-budgets-api-openapi.yml\n  - openapi/aws-cost-explorer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/authentication/amazon-billing-and-cost-management-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Billing
- Cost Management
- Cost Explorer
- Budgets
- Cost Optimization
- FinOps
- Amazon Web Services
---
