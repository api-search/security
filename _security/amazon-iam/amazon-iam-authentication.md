---
api_key_in:
- header
api_specs:
- filename: amazon-iam-openapi.yml
  format: yaml
  label: AWS IAM API
  slug: aws-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/openapi/amazon-iam-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IAM secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IAM
provider_slug: amazon-iam
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: AWS4Auth
  parameter: Authorization
  sources:
  - openapi/amazon-iam-openapi.yml
  type: apiKey
slug: amazon-iam-authentication
source_filename: amazon-iam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iam-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AWS4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-iam-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/authentication/amazon-iam-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Access Management
- Authentication
- Authorization
- Identity
- Security
---
