---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CodePostalPro Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodePostalPro declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CodePostalPro
provider_slug: codepostalpro-com
scheme_count: 3
schemes:
- description: No key needed for up to 1,000 requests a day per IP.
  name: anonymous
  type: none
- description: Free or Pro key sent as X-Api-Key; raises the daily and per-minute quota.
  header: X-Api-Key
  in: header
  name: ApiKeyHeader
  type: apiKey
- description: The same API key may be sent as Authorization Bearer.
  name: BearerKey
  scheme: bearer
  type: http
slug: codepostalpro-com-authentication
source_filename: codepostalpro-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CodePostalPro authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://codepostalpro.com/api/\ndocs: https://codepostalpro.com/api/\nschemes:\n- name: anonymous\n  type: none\n  description: No key needed for up to 1,000 requests a day per IP.\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  header: X-Api-Key\n  description: Free or Pro key sent as X-Api-Key; raises the daily and per-minute quota.\n- name: BearerKey\n  type: http\n  scheme: bearer\n  description: The same API key may be sent as Authorization Bearer.\nkey_issuance:\n  description: A free key is issued by POST /v1/keys with a JSON body containing an email. One key per email — posting again returns the same key. GET /v1/keys/me shows plan and today's usage (documented; not called).\n  note: Key issuance endpoint read from the docs only; it was not exercised.\nmcp:\n  endpoint: https://api.codepostalpro.com/mcp\n  description: Pass an API key as X-Api-Key for the higher limits; quotas\
  \ apply per tool call.\n"
source_yaml_url: https://artifacts.apis.io/codepostalpro-com/authentication/codepostalpro-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Postal Codes
- ZIP Codes
- Geocoding
- Geographic Data
- Open Data
- MCP
---
