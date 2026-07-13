---
api_key_in:
- header
api_specs:
- filename: amazon-polly-openapi.yml
  format: yaml
  label: Amazon Polly API
  slug: amazon-polly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/openapi/amazon-polly-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Polly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Polly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Polly
provider_slug: amazon-polly
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-polly-openapi-original.yaml
  - openapi/amazon-polly-openapi.yml
  type: apiKey
slug: amazon-polly-authentication
source_filename: amazon-polly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-polly-openapi-original.yaml, openapi/amazon-polly-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-polly-openapi-original.yaml\n  - openapi/amazon-polly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/authentication/amazon-polly-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Machine Learning
- Speech Synthesis
- Text-To-Speech
- TTS
- Voice
- SSML
- Neural Engine
- Generative AI
---
