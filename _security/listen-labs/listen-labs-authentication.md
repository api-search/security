---
api_key_in:
- header
api_specs:
- filename: listen-labs-study-data-openapi.json
  format: json
  label: Listen Labs Public API — Study Data
  slug: study-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listen-labs/refs/heads/main/openapi/listen-labs-study-data-openapi.json
- filename: listen-labs-v2-openapi.yml
  format: yaml
  label: Listen Labs Public API v2
  slug: v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listen-labs/refs/heads/main/openapi/listen-labs-v2-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Listen Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Listen Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Listen Labs
provider_slug: listen-labs
scheme_count: 1
schemes:
- description: API key scoped to a single organization. Contact support@listenlabs.ai to request one.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/listen-labs-study-data-openapi.json
  - openapi/listen-labs-v2-openapi.yml
  type: apiKey
slug: listen-labs-authentication
source_filename: listen-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/listen-labs-study-data-openapi.json, openapi/listen-labs-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key scoped to a single organization. Contact support@listenlabs.ai to request\n    one.\n  sources:\n  - openapi/listen-labs-study-data-openapi.json\n  - openapi/listen-labs-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listen-labs/refs/heads/main/authentication/listen-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Market Research
- Customer Research
- User Interviews
- Surveys
- Qualitative Research
- Voice AI
- Insights
- Agents
---
