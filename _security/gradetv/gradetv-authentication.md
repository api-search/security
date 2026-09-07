---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Grade API
  slug: grade-api
  spec_type: OpenAPI
  url: https://gradetv.net/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gradetv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grade secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Grade
provider_slug: gradetv
scheme_count: 1
schemes:
- description: ipt_… (guest) ou iptk_… (API key)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gradetv-openapi.json
  type: http
slug: gradetv-authentication
source_filename: gradetv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/gradetv-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: ipt_… (guest) ou iptk_… (API key)\n  sources:\n  - openapi/gradetv-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradetv/refs/heads/main/authentication/gradetv-authentication.yml
summary_line: http · 1 scheme
tags:
- IPTV
- Streaming
- Live TV
- Live Radio
- Media Catalog
- Broadcast Metadata
- EPG
- TV Guide
- Content Aggregation
- Agent-native
- MCP
- x402
- Micropayments
- Brazil
---
