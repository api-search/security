---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cascade-industries-balance-api-openapi.yml
  format: yaml
  label: Cascade Balance API
  slug: cascade-industries-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cascade-industries/openapi/cascade-industries-balance-api-openapi.yml
- filename: cascade-industries-device-api-openapi.yml
  format: yaml
  label: Cascade Device API
  slug: cascade-industries-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cascade-industries/openapi/cascade-industries-device-api-openapi.yml
- filename: cascade-industries-forecast-api-openapi.yml
  format: yaml
  label: Cascade Forecast API
  slug: cascade-industries-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cascade-industries/openapi/cascade-industries-forecast-api-openapi.yml
- filename: cascade-industries-models-api-openapi.yml
  format: yaml
  label: Cascade Models API
  slug: cascade-industries-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cascade-industries/openapi/cascade-industries-models-api-openapi.yml
- filename: cascade-industries-usage-api-openapi.yml
  format: yaml
  label: Cascade Usage API
  slug: cascade-industries-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cascade-industries/openapi/cascade-industries-usage-api-openapi.yml
auth_types:
- http
- oauth2-device-flow
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cascade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cascade secures its APIs with http and oauth2-device-flow across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cascade
provider_slug: cascade-industries
scheme_count: 3
schemes:
- bearerFormat: pc_live_...
  description: Ephemeris application API key. "Every v1 endpoint requires an Ephemeris API key in the Authorization header. Store keys server-side and revoke any key that may have been exposed." "API keys use the pc_live_ prefix and are shown once when created."
  header: 'Authorization: Bearer pc_live_your_key'
  key_management: Keys are created and revoked on the dashboard API keys page (https://ephemeris.cascade.industries/dashboard/api-keys).
  name: apiKey
  scheme: bearer
  sources:
  - openapi/cascade-industries-openapi.yml
  - https://ephemeris.cascade.industries/docs
  type: http
- description: '"A CLI or agent can get a key without anyone copying it: the OAuth 2.0 device flow (RFC 8628), the same as gh auth login." The flow issues an Ephemeris API key (pc_live_...) rather than an OAuth access token; "Codes expire after 10 minutes."'
  endpoints:
    device_authorization: POST /api/v1/device/code (startDeviceLogin)
    token: POST /api/v1/device/token (pollDeviceLogin)
  flow: device_code
  name: deviceFlow
  note: Read from the docs only; these endpoints were not called. The OpenAPI does not declare this as an oauth2 securityScheme; startDeviceLogin and pollDeviceLogin are modelled as plain operations.
  polling_errors:
  - authorization_pending
  - slow_down
  scopes: none documented
  sources:
  - https://ephemeris.cascade.industries/docs
  standard: RFC 8628
  type: oauth2
- description: The remote MCP server at https://ephemeris.cascade.industries/api/mcp uses the same API key as a bearer header. "OAuth sign-in for one-click connectors is planned; today every client needs a key."
  name: mcp
  scheme: bearer
  sources:
  - https://ephemeris.cascade.industries/docs
  type: http
slug: cascade-industries-authentication
source_filename: cascade-industries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://ephemeris.cascade.industries/docs\ndocs: https://ephemeris.cascade.industries/docs#authentication\nsummary:\n  types:\n  - http\n  - oauth2-device-flow\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: pc_live_...\n  header: 'Authorization: Bearer pc_live_your_key'\n  description: Ephemeris application API key. \"Every v1 endpoint requires an Ephemeris API key in the Authorization header. Store keys server-side and revoke any key that may have been exposed.\" \"API keys use the pc_live_ prefix and are shown once when created.\"\n  key_management: Keys are created and revoked on the dashboard API keys page (https://ephemeris.cascade.industries/dashboard/api-keys).\n  sources:\n  - openapi/cascade-industries-openapi.yml\n  - https://ephemeris.cascade.industries/docs\n- name: deviceFlow\n  type: oauth2\n  flow: device_code\n  standard: RFC 8628\n  description: '\"A CLI or agent can get a key without\
  \ anyone copying it: the OAuth 2.0 device flow (RFC 8628), the same as gh auth login.\" The flow issues an Ephemeris API key (pc_live_...) rather than an OAuth access token; \"Codes expire after 10 minutes.\"'\n  endpoints:\n    device_authorization: POST /api/v1/device/code (startDeviceLogin)\n    token: POST /api/v1/device/token (pollDeviceLogin)\n  polling_errors: [authorization_pending, slow_down]\n  scopes: none documented\n  note: Read from the docs only; these endpoints were not called. The OpenAPI does not declare this as an oauth2 securityScheme; startDeviceLogin and pollDeviceLogin are modelled as plain operations.\n  sources:\n  - https://ephemeris.cascade.industries/docs\n- name: mcp\n  type: http\n  scheme: bearer\n  description: The remote MCP server at https://ephemeris.cascade.industries/api/mcp uses the same API key as a bearer header. \"OAuth sign-in for one-click connectors is planned; today every client needs a key.\"\n  sources:\n  - https://ephemeris.cascade.industries/docs\n"
source_yaml_url: https://artifacts.apis.io/cascade-industries/authentication/cascade-industries-authentication.yml
summary_line: http/oauth2-device-flow · 3 schemes
tags:
- Company
- Time Series
- Forecasting
- Artificial Intelligence
- Machine Learning
- Foundation Models
- MCP
- Benchmarks
---
