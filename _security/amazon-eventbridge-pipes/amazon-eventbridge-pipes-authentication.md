---
api_key_in:
- header
api_specs:
- filename: amazon-eventbridge-pipes-openapi.yml
  format: yaml
  label: Amazon EventBridge Pipes API
  slug: amazon-eventbridge-pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/openapi/amazon-eventbridge-pipes-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Eventbridge Pipes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EventBridge Pipes secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-eventbridge-pipes-openapi.yml
  type: apiKey
slug: amazon-eventbridge-pipes-authentication
source_filename: amazon-eventbridge-pipes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-eventbridge-pipes-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-eventbridge-pipes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/authentication/amazon-eventbridge-pipes-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
---
