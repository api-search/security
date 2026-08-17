---
api_key_in:
- header
api_specs:
- filename: on24-client-level-analytics-openapi.yml
  format: yaml
  label: ON24 Platform API
  slug: on24-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/on24/refs/heads/main/openapi/on24-client-level-analytics-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: On24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: On24 secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: On24
provider_slug: on24
scheme_count: 2
schemes:
- description: API access token key issued by the ON24 platform. Must be supplied together with AccessTokenSecret.
  in: header
  key_name: AccessTokenKey
  name: AccessTokenKey
  type: apiKey
- description: API access token secret corresponding to the AccessTokenKey. Must be supplied together with AccessTokenKey.
  in: header
  key_name: AccessTokenSecret
  name: AccessTokenSecret
  type: apiKey
slug: on24-authentication
source_filename: on24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.on24.com/v2/openapi.json (components.securitySchemes, now harvested), https://apidoc.on24.com/,\n  and https://support.on24.com/hc/en-us/articles/21420840502555-API-Tokens\ndocs: https://support.on24.com/hc/en-us/articles/21420840502555-API-Tokens\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: 'ON24 authenticates every request with a PAIR of apiKey headers, AccessTokenKey and AccessTokenSecret.\n    Both must be supplied together — the spec description says so explicitly and a live probe confirms it (401 \"Header\n    must contain both accessTokenKey and accessTokenSecret\"). Header names are matched case-insensitively: the spec\n    declares AccessTokenKey/AccessTokenSecret while the operation-level parameters and ON24''s own curl example\n    use lowercase accesstokenkey/accesstokensecret. A numeric client id in the URL path scopes every call. There\n    is no OAuth 2.0 / OIDC surface and\
  \ therefore no scope model.'\nschemes:\n- name: AccessTokenKey\n  type: apiKey\n  in: header\n  key_name: AccessTokenKey\n  description: API access token key issued by the ON24 platform. Must be supplied together with AccessTokenSecret.\n- name: AccessTokenSecret\n  type: apiKey\n  in: header\n  key_name: AccessTokenSecret\n  description: API access token secret corresponding to the AccessTokenKey. Must be supplied together with AccessTokenKey.\napplied:\n  global: true\n  operations_covered: 67\n  operations_total: 67\n  note: Declared as a root-level `security` requirement, so all 67 operations are covered.\nclient_scope:\n  in: path\n  parameter: clientId\n  description: Numeric ON24 client (account) id scoping every call; forms part of the base path https://api.on24.com/v2/client/{clientId}/...\nprovisioning:\n  gated: true\n  requires_product: Connect\n  permission: Manage Integrations\n  ui_path: Platform Tools > Integrations > API Tokens\n  access_choice: All endpoints (selected\
  \ at provisioning time; the token is bound to a chosen platform login)\n  one_per_login: Provisioning is only enabled when no token already exists for that producer login.\n  notes: 'Credentials are sales/contract-gated: the contract must include \"Connect\" before a token can be provisioned\n    at all. Ten operations additionally require the Elite tier (403 \"The client id is not an Elite user\").'\n  source: https://support.on24.com/hc/en-us/articles/21420840502555-API-Tokens\nrotation:\n  inactivity_disable_days: 60\n  warning_emails: true\n  re_enable: self-service in the platform\n  notes: Tokens unused for 60 days are automatically disabled; the counter resets on any activity.\ntransport:\n  server_to_server_only: true\n  notes: ON24 states all API calls must be performed server to server and not client-side from a browser.\noauth2: false\noidc: false\nmtls: false\nfailure_modes:\n- status: 401\n  condition: One or both headers missing\n  message: Header must contain both accessTokenKey\
  \ and accessTokenSecret.\n- status: 401\n  condition: Token pair wrong, invalid, not found, or deactivated\n  message: AccessTokenKey and AccessTokenSecret are wrong or invalid.\n- status: 403\n  condition: Token valid but not entitled to the client/endpoint\n  message: You do not have permission to perform the requested operation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/on24/refs/heads/main/authentication/on24-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Webinars
- Virtual Events
- Digital Engagement
- Marketing
- Analytics
- Event Management
- Martech
---
