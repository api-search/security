---
api_key_in:
- header
api_specs:
- filename: amazon-cloudformation-openapi.yml
  format: yaml
  label: Amazon CloudFormation API
  slug: amazon-cloudformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/openapi/amazon-cloudformation-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Cloudformation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CloudFormation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_auth
  parameter: Authorization
  sources:
  - openapi/amazon-cloudformation-openapi.yml
  type: apiKey
slug: amazon-cloudformation-authentication
source_filename: amazon-cloudformation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-cloudformation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-cloudformation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/authentication/amazon-cloudformation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
---
