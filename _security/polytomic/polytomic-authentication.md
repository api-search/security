---
api_key_in: []
api_specs:
- filename: polytomic-openapi.json
  format: json
  label: Polytomic API
  slug: polytomic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polytomic/refs/heads/main/openapi/polytomic-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Polytomic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polytomic secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Polytomic
provider_slug: polytomic
scheme_count: 2
schemes:
- description: Bearer user API key
  name: bearerUserAPIKey
  scheme: bearer
  sources:
  - openapi/polytomic-openapi.json
  type: http
- description: Basic [example key] API key
  name: orgScopedAPIKey
  scheme: basic
  sources:
  - openapi/polytomic-openapi.json
  type: http
slug: polytomic-authentication
source_filename: polytomic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polytomic-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerUserAPIKey\n  type: http\n  scheme: bearer\n  description: Bearer user API key\n  sources:\n  - openapi/polytomic-openapi.json\n- name: orgScopedAPIKey\n  type: http\n  scheme: basic\n  description: Basic [example key] API key\n  sources:\n  - openapi/polytomic-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polytomic/refs/heads/main/authentication/polytomic-authentication.yml
summary_line: http · 2 schemes
tags:
- Data Integration
- Reverse ETL
- Unified API
- ELT
- Data Sync
---
