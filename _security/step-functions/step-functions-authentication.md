---
api_key_in:
- header
api_specs:
- filename: step-functions-openapi.yml
  format: yaml
  label: AWS Step Functions API
  slug: step-functions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/step-functions/refs/heads/main/openapi/step-functions-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Step Functions Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Step Functions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Step Functions
provider_slug: step-functions
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The authorization header includes the credential, signed headers, and signature. Use AWS SDK for automatic signing.
  in: header
  name: awsSigV4
  parameter: Authorization
  sources:
  - openapi/step-functions-openapi.yml
  type: apiKey
slug: step-functions-authentication
source_filename: step-functions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/step-functions-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The authorization header includes the credential, signed\n    headers, and signature. Use AWS SDK for automatic signing.\n  sources:\n  - openapi/step-functions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/step-functions/refs/heads/main/authentication/step-functions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Composition
- Serverless Orchestration
- Workflow
- State Machine
- Automation
---
