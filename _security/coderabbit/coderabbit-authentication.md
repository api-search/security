---
api_key_in:
- header
api_specs:
- filename: coderabbit-openapi.yml
  format: yaml
  label: CodeRabbit Reports API
  slug: coderabbit-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coderabbit/refs/heads/main/openapi/coderabbit-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coderabbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeRabbit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CodeRabbit
provider_slug: coderabbit
scheme_count: 1
schemes:
- description: CodeRabbit API key (format cr-xxxxxxxxxx), generated from the CodeRabbit organization settings and passed in the x-coderabbitai-api-key header.
  in: header
  name: apiKeyAuth
  parameter: x-coderabbitai-api-key
  sources:
  - openapi/coderabbit-openapi.yml
  type: apiKey
slug: coderabbit-authentication
source_filename: coderabbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coderabbit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-coderabbitai-api-key\n  description: CodeRabbit API key (format cr-xxxxxxxxxx), generated from the CodeRabbit organization\n    settings and passed in the x-coderabbitai-api-key header.\n  sources:\n  - openapi/coderabbit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coderabbit/refs/heads/main/authentication/coderabbit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Code Review
- Developer Tools
- Pull Requests
- DevOps
---
