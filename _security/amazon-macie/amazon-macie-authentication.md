---
api_key_in:
- header
api_specs:
- filename: amazon-macie-openapi-original.yaml
  format: yaml
  label: Amazon Macie API
  slug: amazon-macie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/openapi/amazon-macie-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Macie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Macie secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Macie
provider_slug: amazon-macie
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-macie-openapi-original.yaml
  type: apiKey
slug: amazon-macie-authentication
source_filename: amazon-macie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-macie-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-macie-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/authentication/amazon-macie-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
---
