---
api_key_in:
- header
api_specs:
- filename: amazon-step-functions.yaml
  format: yaml
  label: Amazon Step Functions API
  slug: amazon-step-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/openapi/amazon-step-functions.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Step Functions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Step Functions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4Auth
  parameter: Authorization
  sources:
  - openapi/amazon-step-functions-openapi.yml
  - openapi/amazon-step-functions.yaml
  type: apiKey
slug: amazon-step-functions-authentication
source_filename: amazon-step-functions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-step-functions-openapi.yml, openapi/amazon-step-functions.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-step-functions-openapi.yml\n  - openapi/amazon-step-functions.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/authentication/amazon-step-functions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
---
