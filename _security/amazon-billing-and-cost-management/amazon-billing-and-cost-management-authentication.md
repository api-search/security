---
api_key_in:
- header
api_specs:
- filename: amazon-billing-and-cost-management-anomaly-detection-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Anomaly Detection API
  slug: amazon-billing-and-cost-management-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-anomaly-detection-api-openapi.yml
- filename: amazon-billing-and-cost-management-budget-actions-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Budget Actions API
  slug: amazon-billing-and-cost-management-budget-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-budget-actions-api-openapi.yml
- filename: amazon-billing-and-cost-management-budgets-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Budgets API
  slug: amazon-billing-and-cost-management-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-budgets-api-openapi.yml
- filename: amazon-billing-and-cost-management-cost-and-usage-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Cost And Usage API
  slug: amazon-billing-and-cost-management-cost-and-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-cost-and-usage-api-openapi.yml
- filename: amazon-billing-and-cost-management-cost-categories-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Cost Categories API
  slug: amazon-billing-and-cost-management-cost-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-cost-categories-api-openapi.yml
- filename: amazon-billing-and-cost-management-forecasting-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Forecasting API
  slug: amazon-billing-and-cost-management-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-forecasting-api-openapi.yml
- filename: amazon-billing-and-cost-management-notifications-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Notifications API
  slug: amazon-billing-and-cost-management-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-notifications-api-openapi.yml
- filename: amazon-billing-and-cost-management-recommendations-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Recommendations API
  slug: amazon-billing-and-cost-management-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-recommendations-api-openapi.yml
- filename: amazon-billing-and-cost-management-tags-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Tags API
  slug: amazon-billing-and-cost-management-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-tags-api-openapi.yml
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
