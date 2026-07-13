---
api_key_in:
- header
api_specs:
- filename: amazon-fargate-openapi.yml
  format: yaml
  label: Amazon Fargate API
  slug: amazon-fargate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/openapi/amazon-fargate-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Fargate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Fargate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Fargate
provider_slug: amazon-fargate
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Include the Authorization header with the AWS4-HMAC-SHA256 signing algorithm.
  in: header
  name: aws_signature_v4
  parameter: Authorization
  sources:
  - openapi/amazon-fargate-openapi.yml
  type: apiKey
slug: amazon-fargate-authentication
source_filename: amazon-fargate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-fargate-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. Include the Authorization header with\n    the AWS4-HMAC-SHA256 signing algorithm.\n  sources:\n  - openapi/amazon-fargate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/authentication/amazon-fargate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
---
