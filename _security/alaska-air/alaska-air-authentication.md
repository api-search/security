---
api_key_in:
- header
api_specs:
- filename: alaska-air-flight-status-openapi.yaml
  format: yaml
  label: Alaska Airlines Flight Status API
  slug: flight-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-flight-status-openapi.yaml
- filename: alaska-air-flight-schedules-openapi.yaml
  format: yaml
  label: Alaska Airlines Flight Schedules API
  slug: flight-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-flight-schedules-openapi.yaml
- filename: alaska-air-cargo-openapi.yaml
  format: yaml
  label: Alaska Air Cargo API
  slug: cargo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-cargo-openapi.yaml
- filename: alaska-air-mileage-plan-openapi.yaml
  format: yaml
  label: Alaska Airlines Mileage Plan API
  slug: mileage-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-mileage-plan-openapi.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Alaska Air Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Alaska Airlines secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Alaska Airlines
provider_slug: alaska-air
scheme_count: 2
schemes:
- description: API subscription key for Alaska Air Cargo
  in: header
  name: ApiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/alaska-air-cargo-openapi.yaml
  - openapi/alaska-air-flight-schedules-openapi.yaml
  - openapi/alaska-air-flight-status-openapi.yaml
  type: apiKey
- description: OAuth 2.0 for Mileage Plan partner API access
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.alaskaair.com/oauth/token
  name: OAuth2
  sources:
  - openapi/alaska-air-mileage-plan-openapi.yaml
  type: oauth2
slug: alaska-air-authentication
source_filename: alaska-air-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alaska-air-cargo-openapi.yaml, openapi/alaska-air-flight-schedules-openapi.yaml,\n  openapi/alaska-air-flight-status-openapi.yaml, openapi/alaska-air-mileage-plan-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: API subscription key for Alaska Air Cargo\n  sources:\n  - openapi/alaska-air-cargo-openapi.yaml\n  - openapi/alaska-air-flight-schedules-openapi.yaml\n  - openapi/alaska-air-flight-status-openapi.yaml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.alaskaair.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 for Mileage Plan partner API access\n  sources:\n  - openapi/alaska-air-mileage-plan-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/authentication/alaska-air-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
- Fortune 500
---
