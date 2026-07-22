---
api_key_in: []
api_specs:
- filename: standard-metrics-main-openapi.json
  format: json
  label: Standard Metrics API
  slug: standard-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-main-openapi.json
- filename: standard-metrics-investment-data-openapi.json
  format: json
  label: Standard Metrics Investment Data API
  slug: standard-metrics-investment-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-investment-data-openapi.json
auth_types:
- oauth2
- http
description: 'Standard Metrics authenticates with OAuth2 client-credentials. A firm admin creates an OAuth application in Developer Settings, producing a client_id and client_secret. Those are Basic-auth-encoded and POSTed to the token endpoint (grant_type=client_credentials) to obtain a short-lived Bearer JWT (expires_in 3600s), which is then sent as ''Authorization: Bearer <token>'' on every API request. Per-key data access is governed by admin-configured user permissions.'
kind: authentication
layout: security
method: searched
name: Standard Metrics Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Standard Metrics secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Standard Metrics
provider_slug: standard-metrics
scheme_count: 3
schemes:
- flow: clientCredentials
  name: OAuth2 Client Credentials
  note: client_id/client_secret exchanged (Basic auth) for a Bearer access token.
  scopes:
  - read
  - write
  - all
  sources:
  - https://docs.standardmetrics.io/api-reference/setting-up
  tokenUrl: https://api.standardmetrics.io/o/token/
  type: oauth2
- name: basicAuth
  note: Used only on the token endpoint (client_id:client_secret) to obtain a Bearer token.
  scheme: basic
  sources:
  - openapi/standard-metrics-auth-openapi.json
  type: http
- bearerFormat: JWT
  name: BearerAuth
  note: Applied to all data endpoints across the main and investment-data APIs.
  scheme: bearer
  sources:
  - openapi/standard-metrics-main-openapi.json
  - openapi/standard-metrics-investment-data-openapi.json
  type: http
slug: standard-metrics-authentication
source_filename: standard-metrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.standardmetrics.io/api-reference/setting-up\ndocs: https://docs.standardmetrics.io/guides/initialsetup\ndescription: >-\n  Standard Metrics authenticates with OAuth2 client-credentials. A firm admin creates an\n  OAuth application in Developer Settings, producing a client_id and client_secret. Those\n  are Basic-auth-encoded and POSTed to the token endpoint (grant_type=client_credentials)\n  to obtain a short-lived Bearer JWT (expires_in 3600s), which is then sent as\n  'Authorization: Bearer <token>' on every API request. Per-key data access is governed by\n  admin-configured user permissions.\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  bearer_format: JWT\n  token_endpoint: https://api.standardmetrics.io/o/token/\n  token_ttl_seconds: 3600\nschemes:\n- name: OAuth2 Client Credentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://api.standardmetrics.io/o/token/\n\
  \  scopes: [read, write, all]\n  note: client_id/client_secret exchanged (Basic auth) for a Bearer access token.\n  sources: [https://docs.standardmetrics.io/api-reference/setting-up]\n- name: basicAuth\n  type: http\n  scheme: basic\n  note: Used only on the token endpoint (client_id:client_secret) to obtain a Bearer token.\n  sources: [openapi/standard-metrics-auth-openapi.json]\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  note: Applied to all data endpoints across the main and investment-data APIs.\n  sources:\n  - openapi/standard-metrics-main-openapi.json\n  - openapi/standard-metrics-investment-data-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/authentication/standard-metrics-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Venture Capital
- Private Equity
- Portfolio Management
- Financial Data
- Investment Data
- Cap Table
- Metrics
- Reporting
- MCP
---
