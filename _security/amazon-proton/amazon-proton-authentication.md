---
api_key_in:
- header
api_specs:
- filename: amazon-proton-openapi-original.yaml
  format: yaml
  label: AWS Proton API
  slug: aws-proton-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/openapi/amazon-proton-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Proton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Proton secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Proton
provider_slug: amazon-proton
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-proton-openapi-original.yaml
  type: apiKey
slug: amazon-proton-authentication
source_filename: amazon-proton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-proton-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-proton-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/authentication/amazon-proton-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
---
