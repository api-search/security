---
api_key_in:
- header
api_specs:
- filename: turvo-accounts-api-openapi.yml
  format: yaml
  label: Turvo Accounts API
  slug: turvo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-accounts-api-openapi.yml
- filename: turvo-authentication-api-openapi.yml
  format: yaml
  label: Turvo Authentication API
  slug: turvo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-authentication-api-openapi.yml
- filename: turvo-carriers-api-openapi.yml
  format: yaml
  label: Turvo Carriers API
  slug: turvo-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-carriers-api-openapi.yml
- filename: turvo-locations-api-openapi.yml
  format: yaml
  label: Turvo Locations API
  slug: turvo-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-locations-api-openapi.yml
- filename: turvo-orders-api-openapi.yml
  format: yaml
  label: Turvo Orders API
  slug: turvo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-orders-api-openapi.yml
- filename: turvo-shipments-api-openapi.yml
  format: yaml
  label: Turvo Shipments API
  slug: turvo-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-shipments-api-openapi.yml
- filename: turvo-tracking-api-openapi.yml
  format: yaml
  label: Turvo Tracking API
  slug: turvo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-tracking-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Turvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turvo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Turvo
provider_slug: turvo
scheme_count: 2
schemes:
- description: 'OAuth 2.0 Bearer access token obtained from POST /oauth/token. Passed as Authorization: Bearer [example key]'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/turvo-openapi.yml
  type: http
- description: Per-tenant API key from the Turvo tenant API profile, sent on every request.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/turvo-openapi.yml
  type: apiKey
slug: turvo-authentication
source_filename: turvo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/turvo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 Bearer access token obtained from POST /oauth/token. Passed as Authorization:\n    Bearer [example key]'\n  sources:\n  - openapi/turvo-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Per-tenant API key from the Turvo tenant API profile, sent on every request.\n  sources:\n  - openapi/turvo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/authentication/turvo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Logistics
- Transportation Management System
- TMS
- Supply Chain
- Freight
- Shipments
- Carriers
---
