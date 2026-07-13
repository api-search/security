---
api_key_in:
- header
api_specs:
- filename: aws-step-functions-openapi.json
  format: json
  label: AWS Step Functions
  slug: aws-step-functions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Step Functions Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Step Functions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Step Functions
provider_slug: aws-step-functions
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/aws-step-functions-openapi.json
  type: apiKey
slug: aws-step-functions-authentication
source_filename: aws-step-functions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-step-functions-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/aws-step-functions-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/authentication/aws-step-functions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- iPaaS
- Orchestration
- Serverless
---
