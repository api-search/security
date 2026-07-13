---
api_key_in:
- header
api_specs:
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Collection API
  slug: gameanalytics-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Metrics API
  slug: gameanalytics-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Organization API
  slug: gameanalytics-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gameanalytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: GameAnalytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GameAnalytics
provider_slug: gameanalytics
scheme_count: 2
schemes:
- description: Base64-encoded HMAC-SHA256 digest of the raw (optionally gzipped) request body, keyed with the game's secret key. Used by the Collection API.
  in: header
  name: hmacAuth
  parameter: Authorization
  sources:
  - openapi/gameanalytics-openapi.yml
  type: apiKey
- description: API key generated in the GameAnalytics dashboard. The Metrics API uses the `X-API-Key` header; the Organization API uses an equivalent API-key header.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/gameanalytics-openapi.yml
  type: apiKey
slug: gameanalytics-authentication
source_filename: gameanalytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gameanalytics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmacAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Base64-encoded HMAC-SHA256 digest of the raw (optionally gzipped) request body,\n    keyed with the game's secret key. Used by the Collection API.\n  sources:\n  - openapi/gameanalytics-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key generated in the GameAnalytics dashboard. The Metrics API uses the `X-API-Key`\n    header; the Organization API uses an equivalent API-key header.\n  sources:\n  - openapi/gameanalytics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/authentication/gameanalytics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analytics
- Games
- Gaming
- Player Behavior
- Retention
- Monetization
- Ad Analytics
- Telemetry
---
