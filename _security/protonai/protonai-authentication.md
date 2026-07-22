---
api_key_in:
- header
api_specs:
- filename: protonai-openapi.yml
  format: yaml
  label: Proton API
  slug: proton-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Protonai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proton.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Proton.ai
provider_slug: protonai
scheme_count: 1
schemes:
- description: Static API key supplied by Proton at integration onboarding.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/protonai-openapi.yml
  type: apiKey
slug: protonai-authentication
source_filename: protonai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/protonai-openapi.yml\ndocs: https://api.proton.ai/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Auth is a single static API key sent in the X-Api-Key header, supplied by\n    Proton at the start of an integration (no dynamic generation or refresh).\n    Requests are additionally scoped by an X-Company tenant header and an\n    optional X-User-Id acting-user header. There is no OAuth surface.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Static API key supplied by Proton at integration onboarding.\n  sources:\n  - openapi/protonai-openapi.yml\nadditional_headers:\n- name: X-Company\n  required: true\n  description: Tenant company slug; also appears as the first path segment (/{company}/...).\n- name: X-User-Id\n  required: false\n  description: Identifies the acting user for attribution on writes and tracking events.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/authentication/protonai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- CRM
- Sales
- Distribution
- Artificial Intelligence
- Recommendations
- B2B
- Wholesale Distribution
---
