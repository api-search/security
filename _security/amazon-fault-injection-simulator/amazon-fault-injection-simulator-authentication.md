---
api_key_in:
- header
api_specs:
- filename: amazon-fis-openapi.yml
  format: yaml
  label: AWS Fault Injection Simulator API
  slug: aws-fis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/openapi/amazon-fis-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Fault Injection Simulator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Fault Injection Simulator secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_signature_v4
  parameter: Authorization
  sources:
  - openapi/amazon-fis-openapi.yml
  type: apiKey
slug: amazon-fault-injection-simulator-authentication
source_filename: amazon-fault-injection-simulator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-fis-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-fis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/authentication/amazon-fault-injection-simulator-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
---
