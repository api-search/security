---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: numbers-online-account-api-openapi.yml
  format: yaml
  label: Numbers Online Account API
  slug: numbers-online-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-account-api-openapi.yml
- filename: numbers-online-community-reporting-api-openapi.yml
  format: yaml
  label: Numbers Online Community reporting API
  slug: numbers-online-community-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-community-reporting-api-openapi.yml
- filename: numbers-online-inbound-api-openapi.yml
  format: yaml
  label: Numbers Online Inbound API
  slug: numbers-online-inbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-inbound-api-openapi.yml
- filename: numbers-online-lookup-api-openapi.yml
  format: yaml
  label: Numbers Online Lookup API
  slug: numbers-online-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-lookup-api-openapi.yml
- filename: numbers-online-mcp-api-openapi.yml
  format: yaml
  label: Numbers Online MCP API
  slug: numbers-online-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-mcp-api-openapi.yml
- filename: numbers-online-msp-api-openapi.yml
  format: yaml
  label: Numbers Online MSP API
  slug: numbers-online-msp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-msp-api-openapi.yml
- filename: numbers-online-outbound-api-openapi.yml
  format: yaml
  label: Numbers Online Outbound API
  slug: numbers-online-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-outbound-api-openapi.yml
- filename: numbers-online-parsing-api-openapi.yml
  format: yaml
  label: Numbers Online Parsing API
  slug: numbers-online-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-parsing-api-openapi.yml
- filename: numbers-online-pbx-api-openapi.yml
  format: yaml
  label: Numbers Online PBX API
  slug: numbers-online-pbx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-pbx-api-openapi.yml
- filename: numbers-online-receipts-api-openapi.yml
  format: yaml
  label: Numbers Online Receipts API
  slug: numbers-online-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-receipts-api-openapi.yml
- filename: numbers-online-reference-api-openapi.yml
  format: yaml
  label: Numbers Online Reference API
  slug: numbers-online-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-reference-api-openapi.yml
- filename: numbers-online-sbc-sip-api-openapi.yml
  format: yaml
  label: Numbers Online SBC / SIP API
  slug: numbers-online-sbc-sip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-sbc-sip-api-openapi.yml
- filename: numbers-online-system-api-openapi.yml
  format: yaml
  label: Numbers Online System API
  slug: numbers-online-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-system-api-openapi.yml
- filename: numbers-online-trust-api-openapi.yml
  format: yaml
  label: Numbers Online Trust API
  slug: numbers-online-trust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-trust-api-openapi.yml
- filename: numbers-online-webhooks-api-openapi.yml
  format: yaml
  label: Numbers Online Webhooks API
  slug: numbers-online-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numbers-online/refs/heads/main/openapi/numbers-online-webhooks-api-openapi.yml
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
