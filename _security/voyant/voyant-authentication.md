---
api_key_in: []
api_specs:
- filename: voyant-openapi-original.json
  format: json
  label: VoyantIO API
  slug: voyantio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voyant/refs/heads/main/openapi/voyant-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Voyant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voyant.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voyant.io
provider_slug: voyant
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/voyant-openapi-original.json
  type: http
slug: voyant-authentication
source_filename: voyant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/voyant-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/voyant-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyant/refs/heads/main/authentication/voyant-authentication.yml
summary_line: http · 1 scheme
tags:
- artificial-intelligence
- context-management
- brand-governance
- product-marketing
- gtm-operations
- marketing-automation
- content-generation
- competitive-intelligence
- semantic-search
- rag
- mcp
- agent-native
- signals
- telemetry
---
