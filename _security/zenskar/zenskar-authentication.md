---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Zenskar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenskar secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zenskar
provider_slug: zenskar
scheme_count: 2
schemes:
- description: Organisation API key passed in the x-api-key header. Created and rotated from the Zenskar dashboard (Settings -> API keys).
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  sources:
  - https://docs.zenskar.com/reference/authentication
  type: apiKey
- bearer_format: JWT
  description: 'JWT bearer token (format eyJ...) accepted by the API / MCP server as `Authorization: Bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://docs.zenskar.com/docs/mcp-reference
  type: http
slug: zenskar-authentication
source_filename: zenskar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.zenskar.com/reference/authentication\ndocs: https://docs.zenskar.com/reference/authentication\nnotes: >-\n  Zenskar's REST API is key-authenticated. API keys are created and managed from\n  the Zenskar dashboard (see https://docs.zenskar.com/docs/how-to-manage-api-keys).\n  The same credential model is used by the Zenskar MCP server, which auto-detects\n  the token type: JWT tokens (format eyJ...) are sent as `Authorization: Bearer <token>`,\n  while API keys are sent via the `x-api-key: <token>` header. Dashboard/console access\n  additionally supports SAML SSO, single sign-on, and two-factor authentication.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  api_key_headers: [x-api-key]\n  http_schemes: [bearer]\n  oauth2_flows: []\n  dashboard_sso: [SAML 2.0, SSO, 2FA]\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Organisation API key\
  \ passed in the x-api-key header. Created and rotated from\n    the Zenskar dashboard (Settings -> API keys).\n  sources: [https://docs.zenskar.com/reference/authentication]\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    JWT bearer token (format eyJ...) accepted by the API / MCP server as\n    `Authorization: Bearer <token>`.\n  sources: [https://docs.zenskar.com/docs/mcp-reference]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenskar/refs/heads/main/authentication/zenskar-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Cloud
- Billing
- Usage-Based Billing
- Revenue Automation
- Subscription Management
- Revenue Recognition
- Invoicing
- FinTech
- Order-to-Cash
- MCP
---
