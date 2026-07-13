---
api_key_in:
- header
api_specs:
- filename: cloudformation-api.yml
  format: yaml
  label: AWS CloudFormation API
  slug: aws-cloudformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-api.yml
- filename: cloud-control-api.yml
  format: yaml
  label: AWS Cloud Control API
  slug: aws-cloud-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloud-control-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudformation Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS CloudFormation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS CloudFormation
provider_slug: cloudformation
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: AWS_Signature_V4
  parameter: Authorization
  sources:
  - openapi/cloud-control-api.yml
  - openapi/cloudformation-api.yml
  type: apiKey
slug: cloudformation-authentication
source_filename: cloudformation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-control-api.yml, openapi/cloudformation-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AWS_Signature_V4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/cloud-control-api.yml\n  - openapi/cloudformation-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/authentication/cloudformation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
---
