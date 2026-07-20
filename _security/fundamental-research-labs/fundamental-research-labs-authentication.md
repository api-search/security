---
api_key_in:
- cookie
api_specs:
- filename: fundamental-research-labs-openapi-original.json
  format: json
  label: Shortcut API
  slug: shortcut-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundamental-research-labs/refs/heads/main/openapi/fundamental-research-labs-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fundamental Research Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fundamental Research Labs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fundamental Research Labs
provider_slug: fundamental-research-labs
scheme_count: 2
schemes:
- bearerFormat: API Key
  description: 'API key in Bearer token format: `Authorization: Bearer [example key]`'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/fundamental-research-labs-openapi-original.json
  type: http
- description: Shortcut web session cookie for credentialed fetch requests. Missing or untrusted Origin headers are rejected.
  in: cookie
  name: shortcutCookie
  parameter: shortcut_access_token
  sources:
  - openapi/fundamental-research-labs-openapi-original.json
  type: apiKey
slug: fundamental-research-labs-authentication
source_filename: fundamental-research-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fundamental-research-labs-openapi-original.json\ndocs: https://shortcut.ai/docs/platform-api\nnotes: 'External callers authenticate with an API key sent as a Bearer token (`Authorization:\n  Bearer [example key]`), created from Settings -> API Keys in Shortcut. First-party Shortcut\n  applications may instead pass the user session/access token as a Bearer token\n  (shortcutSession) or, for trusted Shortcut web origins, via the `shortcut_access_token`\n  cookie (shortcutCookie). `/verify` and webhooks require API-key auth. No OAuth2 or\n  OpenID Connect flows are offered.'\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'API key in Bearer token format: `Authorization: Bearer [example key]`'\n  sources:\n  - openapi/fundamental-research-labs-openapi-original.json\n- name: shortcutCookie\n  type: apiKey\n\
  \  in: cookie\n  parameter: shortcut_access_token\n  description: Shortcut web session cookie for credentialed fetch requests. Missing or untrusted\n    Origin headers are rejected.\n  sources:\n  - openapi/fundamental-research-labs-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundamental-research-labs/refs/heads/main/authentication/fundamental-research-labs-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai
- Artificial Intelligence
- Spreadsheets
- Excel
- Financial Modeling
- Agents
- Automation
- Productivity
- Data Analysis
---
