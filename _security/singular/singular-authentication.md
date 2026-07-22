---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Singular Authentication
name_suffix: Authentication
oauth_flows: []
overview: Singular secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Singular
provider_slug: singular
scheme_count: 1
schemes:
- description: The Singular Reporting API authenticates with an account API key passed as the api_key request parameter. An unauthenticated request to https://api.singular.net/api/v2.0/reporting returns HTTP 401, confirming that credentials are required. The API key is issued per account from the Singular dashboard (Settings > API keys).
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - live-probe:401
  - docs:support.singular.net
  type: apiKey
slug: singular-authentication
source_filename: singular-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.singular.net/hc/en-us + https://api.singular.net/api/v2.0/reporting probe\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: query\n    parameter: api_key\n    description: >-\n      The Singular Reporting API authenticates with an account API key passed as\n      the api_key request parameter. An unauthenticated request to\n      https://api.singular.net/api/v2.0/reporting returns HTTP 401, confirming\n      that credentials are required. The API key is issued per account from the\n      Singular dashboard (Settings > API keys).\n    sources: [live-probe:401, docs:support.singular.net]\nnotes: >-\n  No public OpenAPI/Swagger is served (openapi.json / swagger.json return 404).\n  No OAuth2 or OIDC discovery document is exposed (/.well-known/openid-configuration\n  and /.well-known/oauth-authorization-server return 404), consistent with\
  \ a\n  key-auth model. SDK-side auth (SDK Key) governs the client mobile SDKs and is\n  distinct from the server-side Reporting API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singular/refs/heads/main/authentication/singular-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketing Analytics
- Mobile Attribution
- Attribution
- Marketing
- Advertising
- Analytics
- Mobile Measurement Partner
- SKAdNetwork
- Deep Linking
- Fraud Prevention
- ETL
---
