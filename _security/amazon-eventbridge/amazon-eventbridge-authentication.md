---
api_key_in:
- header
api_specs:
- filename: amazon-eventbridge-openapi.yml
  format: yaml
  label: Amazon EventBridge API
  slug: amazon-eventbridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/openapi/amazon-eventbridge-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Eventbridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EventBridge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-eventbridge-openapi.yml
  type: apiKey
slug: amazon-eventbridge-authentication
source_filename: amazon-eventbridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-eventbridge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-eventbridge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/authentication/amazon-eventbridge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
---
