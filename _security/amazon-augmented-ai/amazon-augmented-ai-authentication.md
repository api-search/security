---
api_key_in:
- header
api_specs:
- filename: amazon-augmented-ai-openapi.yml
  format: yaml
  label: Amazon Augmented AI API
  slug: amazon-augmented-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-augmented-ai/refs/heads/main/openapi/amazon-augmented-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Augmented Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Augmented AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Augmented AI
provider_slug: amazon-augmented-ai
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-augmented-ai-openapi.yml
  type: apiKey
slug: amazon-augmented-ai-authentication
source_filename: amazon-augmented-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-augmented-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-augmented-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-augmented-ai/refs/heads/main/authentication/amazon-augmented-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Augmented AI
- Human In The Loop
- Machine Learning
- AI Review
---
