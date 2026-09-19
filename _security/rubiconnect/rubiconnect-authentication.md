---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: rubiconnect-campaigns-api-openapi.yml
  format: yaml
  label: RubiConnect Campaigns API
  slug: rubiconnect-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-campaigns-api-openapi.yml
- filename: rubiconnect-capabilities-api-openapi.yml
  format: yaml
  label: RubiConnect Capabilities API
  slug: rubiconnect-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-capabilities-api-openapi.yml
- filename: rubiconnect-messages-api-openapi.yml
  format: yaml
  label: RubiConnect Messages API
  slug: rubiconnect-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-messages-api-openapi.yml
- filename: rubiconnect-webhooks-api-openapi.yml
  format: yaml
  label: RubiConnect Webhooks API
  slug: rubiconnect-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Rubiconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: RubiConnect secures its APIs with apiKey, http, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RubiConnect
provider_slug: rubiconnect
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/rubiconnect-openapi.json
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/rubiconnect-openapi.json
  type: http
slug: rubiconnect-authentication
source_filename: rubiconnect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: searched\nsource: >-\n  openapi/rubiconnect-openapi.json (REST schemes) +\n  https://console.rubiconnect.com/.well-known/oauth-authorization-server (MCP OAuth)\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  api_key_prefix: rc_live_\n  oauth:\n    flow: authorization_code\n    pkce: [S256, plain]\n    dynamic_client_registration: true\n    authorization_endpoint: https://console.rubiconnect.com/en/authorize\n    token_endpoint: https://console.rubiconnect.com/api/oauth/token\n    registration_endpoint: https://console.rubiconnect.com/api/oauth/register\n    scopes: [mcp]\n    applies_to: hosted MCP server (not declared in the REST OpenAPI)\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/rubiconnect-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/rubiconnect-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/authentication/rubiconnect-authentication.yml
summary_line: apiKey/http/oauth2 · 2 schemes
tags:
- CPaaS
- Communications APIs
- Business Messaging
- RCS
- WhatsApp Business
- SMS
- Marketing & Campaigns
- Conversational AI
- MCP
- AI Agents
---
