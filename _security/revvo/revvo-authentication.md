---
api_key_in:
- header
api_specs:
- filename: revvo-api-keys-api-openapi.yml
  format: yaml
  label: Revvo Api-keys API
  slug: revvo-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-api-keys-api-openapi.yml
- filename: revvo-auth-api-openapi.yml
  format: yaml
  label: Revvo Auth API
  slug: revvo-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-auth-api-openapi.yml
- filename: revvo-device-api-openapi.yml
  format: yaml
  label: Revvo Device API
  slug: revvo-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-device-api-openapi.yml
- filename: revvo-event-api-openapi.yml
  format: yaml
  label: Revvo Event API
  slug: revvo-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-event-api-openapi.yml
- filename: revvo-fleet-api-openapi.yml
  format: yaml
  label: Revvo Fleet API
  slug: revvo-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-fleet-api-openapi.yml
- filename: revvo-tire-operation-api-openapi.yml
  format: yaml
  label: Revvo Tire Operation API
  slug: revvo-tire-operation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-tire-operation-api-openapi.yml
- filename: revvo-vehicle-api-openapi.yml
  format: yaml
  label: Revvo Vehicle API
  slug: revvo-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-vehicle-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Revvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revvo secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Revvo
provider_slug: revvo
scheme_count: 2
schemes:
- description: Long-lived fleet API key exchanged at POST /auth for a JWT. Provisioned and revoked via getApiKeys / addApiKey / deleteApiKey.
  in: header
  name: apiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/revvo-api-openapi-original.yml
  type: apiKey
  used_by:
  - authToken
- bearerFormat: JWT
  description: 'Short-lived JWT obtained from POST /auth, sent as Authorization: Bearer on every fleet, device, vehicle, event and tire operation.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/revvo-api-openapi-original.yml
  type: http
slug: revvo-authentication
source_filename: revvo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/revvo-api-openapi-original.yml\ndocs: https://api.revvo.ai/v0/swagger-ui\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  flow: two-step\n  notes: >-\n    Revvo uses a two-step credential exchange. Clients present a long-lived\n    API key in the X-API-KEY header to POST /auth, which returns a short-lived\n    JWT (text/plain). That JWT is then sent as an HTTP bearer token\n    (Authorization: Bearer <jwt>) on all other operations. API keys are\n    managed per fleet via the /api-keys/fleet/{fleetId} endpoints.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  used_by:\n  - authToken\n  description: >-\n    Long-lived fleet API key exchanged at POST /auth for a JWT. Provisioned and\n    revoked via getApiKeys / addApiKey / deleteApiKey.\n  sources:\n  - openapi/revvo-api-openapi-original.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ JWT\n  description: >-\n    Short-lived JWT obtained from POST /auth, sent as Authorization: Bearer on\n    every fleet, device, vehicle, event and tire operation.\n  sources:\n  - openapi/revvo-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/authentication/revvo-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Fleet Management
- Transportation
- Tire Management
- TPMS
- Telematics
- IoT
- Logistics
---
