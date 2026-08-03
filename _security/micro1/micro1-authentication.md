---
api_key_in:
- header
api_specs:
- filename: micro1-ai-recruiter-openapi.yml
  format: yaml
  label: micro1 Public API
  slug: micro1-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-ai-recruiter-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Micro1 Authentication
name_suffix: Authentication
oauth_flows: []
overview: micro1 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: micro1
provider_slug: micro1
scheme_count: 1
schemes:
- description: API key to access the API
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/micro1-ai-recruiter-openapi.yml
  type: apiKey
slug: micro1-authentication
source_filename: micro1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/micro1-ai-recruiter-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key to access the API\n  sources:\n  - openapi/micro1-ai-recruiter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/authentication/micro1-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- recruiting
- hiring
- ai-interviews
- talent-assessment
- candidate-screening
- applicant-tracking
- human-resources
- proctoring
- webhooks
- agent-native
- ai-training-data
---
