---
api_key_in: []
api_specs:
- filename: voxco-aicoder-api-openapi.yml
  format: yaml
  label: Voxco AICoder API
  slug: voxco-aicoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-aicoder-api-openapi.yml
- filename: voxco-codebooks-api-openapi.yml
  format: yaml
  label: Voxco Codebooks API
  slug: voxco-codebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-codebooks-api-openapi.yml
- filename: voxco-companies-api-openapi.yml
  format: yaml
  label: Voxco Companies API
  slug: voxco-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-companies-api-openapi.yml
- filename: voxco-exports-api-openapi.yml
  format: yaml
  label: Voxco Exports API
  slug: voxco-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-exports-api-openapi.yml
- filename: voxco-languages-api-openapi.yml
  format: yaml
  label: Voxco Languages API
  slug: voxco-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-languages-api-openapi.yml
- filename: voxco-questions-api-openapi.yml
  format: yaml
  label: Voxco Questions API
  slug: voxco-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-questions-api-openapi.yml
- filename: voxco-responses-api-openapi.yml
  format: yaml
  label: Voxco Responses API
  slug: voxco-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-responses-api-openapi.yml
- filename: voxco-sessions-api-openapi.yml
  format: yaml
  label: Voxco Sessions API
  slug: voxco-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-sessions-api-openapi.yml
- filename: voxco-studies-api-openapi.yml
  format: yaml
  label: Voxco Studies API
  slug: voxco-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-studies-api-openapi.yml
- filename: voxco-studyrespondents-api-openapi.yml
  format: yaml
  label: Voxco StudyRespondents API
  slug: voxco-studyrespondents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-studyrespondents-api-openapi.yml
- filename: voxco-users-api-openapi.yml
  format: yaml
  label: Voxco Users API
  slug: voxco-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Voxco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voxco secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voxco
provider_slug: voxco
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Please enter a valid bearer token.


    It should be in the format "bearer eyJhbGciOiJSU..."


    It will be added to the "Authentication" HTTP header'
  name: Bearer
  scheme: Bearer
  sources:
  - openapi/voxco-ascribe-coder-api-openapi.json
  type: http
slug: voxco-authentication
source_filename: voxco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/voxco-ascribe-coder-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: |-\n    Please enter a valid bearer token.\n\n    It should be in the format \"bearer eyJhbGciOiJSU...\"\n\n    It will be added to the \"Authentication\" HTTP header\n  sources:\n  - openapi/voxco-ascribe-coder-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/authentication/voxco-authentication.yml
summary_line: http · 1 scheme
tags:
- Survey Software
- Market Research
- CATI
- Omnichannel
- Text Analytics
- Data Collection
- Panel Management
---
