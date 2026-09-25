---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: numbers-online-openapi.yml
  format: yaml
  label: Numbers Online Phone Intelligence API
  slug: numbers-online-phone-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Numbers Online Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numbers Online secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Numbers Online
provider_slug: numbers-online
scheme_count: 3
schemes:
- description: API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/numbers-online-openapi.yml
  type: apiKey
- description: Bearer token authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/numbers-online-openapi.yml
  type: http
- description: API key in the `?key=` query param. Accepted by the header-less PBX endpoint GET /api/v1/cid/{number} and by the webhook adapters POST /api/v1/integrations/retell/inbound, POST /api/v1/integrations/vapi/tool, and POST /api/v1/sbc/redirect, whose upstream platforms set only a static webhook URL and cannot send an Authorization/X-API-Key header. The key can leak into access logs — use a dedicated, r
  in: query
  name: CidQueryKeyAuth
  parameter: key
  sources:
  - openapi/numbers-online-openapi.yml
  type: apiKey
slug: numbers-online-authentication
source_filename: numbers-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/numbers-online-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication\n  sources:\n  - openapi/numbers-online-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication\n  sources:\n  - openapi/numbers-online-openapi.yml\n- name: CidQueryKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key in the `?key=` query param. Accepted by the header-less PBX endpoint\n    GET /api/v1/cid/{number} and by the webhook adapters POST /api/v1/integrations/retell/inbound,\n    POST /api/v1/integrations/vapi/tool, and POST /api/v1/sbc/redirect, whose upstream platforms\n    set only a static webhook URL and cannot send an Authorization/X-API-Key header. The key\n    can leak into access logs — use a\
  \ dedicated, r\n  sources:\n  - openapi/numbers-online-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/authentication/numbers-online-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Phone Intelligence
- Caller ID
- CNAM
- Reverse Phone Lookup
- Spam Detection
- Do Not Call
- Telephony
- STIR/SHAKEN
- MCP
- Agent-Native
- Compliance
- Company
- A2A
---
