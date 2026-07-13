---
api_key_in:
- header
api_specs:
- filename: amazon-batch-openapi.yml
  format: yaml
  label: Amazon Batch API
  slug: amazon-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-batch/refs/heads/main/openapi/amazon-batch-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Batch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Batch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Batch
provider_slug: amazon-batch
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-batch-openapi.yml
  type: apiKey
slug: amazon-batch-authentication
source_filename: amazon-batch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-batch-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-batch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-batch/refs/heads/main/authentication/amazon-batch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Batch Computing
- Compute
- Containers
- HPC
- Job Scheduling
- Serverless
- Fargate
- EKS
- Spot Instances
---
