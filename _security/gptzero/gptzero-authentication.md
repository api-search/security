---
api_key_in:
- header
api_specs:
- filename: gptzero-openapi-original.json
  format: json
  label: GPTZero API
  slug: gptzero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gptzero/refs/heads/main/openapi/gptzero-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gptzero Authentication
name_suffix: Authentication
oauth_flows: []
overview: GPTZero secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GPTZero
provider_slug: gptzero
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/gptzero-openapi-original.json
  type: apiKey
slug: gptzero-authentication
source_filename: gptzero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/gptzero-openapi-original.json\ndocs: https://app.gptzero.me/app/api\ndocs_note: API keys are generated in the GPTZero dashboard (app.gptzero.me/app/api) and sent in the X-API-Key request header. Keys can be rotated per environment. API access requires the Professional plan.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/gptzero-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gptzero/refs/heads/main/authentication/gptzero-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- AI Detection
- Content Moderation
- Machine Learning
- Text Analysis
- Natural Language Processing
- Education
---
