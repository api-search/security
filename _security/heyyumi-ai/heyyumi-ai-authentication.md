---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: heyyumi-ai-categories-api-openapi.yml
  format: yaml
  label: Heyyumi AI Categories API
  slug: heyyumi-ai-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyyumi-ai/openapi/heyyumi-ai-categories-api-openapi.yml
- filename: heyyumi-ai-live-status-api-openapi.yml
  format: yaml
  label: Heyyumi AI Live Status API
  slug: heyyumi-ai-live-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyyumi-ai/openapi/heyyumi-ai-live-status-api-openapi.yml
- filename: heyyumi-ai-meta-api-openapi.yml
  format: yaml
  label: Heyyumi AI Meta API
  slug: heyyumi-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyyumi-ai/openapi/heyyumi-ai-meta-api-openapi.yml
- filename: heyyumi-ai-places-api-openapi.yml
  format: yaml
  label: Heyyumi AI Places API
  slug: heyyumi-ai-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyyumi-ai/openapi/heyyumi-ai-places-api-openapi.yml
- filename: heyyumi-ai-regions-api-openapi.yml
  format: yaml
  label: Heyyumi AI Regions API
  slug: heyyumi-ai-regions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyyumi-ai/openapi/heyyumi-ai-regions-api-openapi.yml
- filename: heyyumi-ai-reservations-api-openapi.yml
  format: yaml
  label: Heyyumi AI Reservations API
  slug: heyyumi-ai-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyyumi-ai/openapi/heyyumi-ai-reservations-api-openapi.yml
- filename: heyyumi-ai-stats-api-openapi.yml
  format: yaml
  label: Heyyumi AI Stats API
  slug: heyyumi-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyyumi-ai/openapi/heyyumi-ai-stats-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Heyyumi AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heyyumi AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Heyyumi AI
provider_slug: heyyumi-ai
scheme_count: 2
schemes:
- description: 'Preferred: Authorization: Bearer <API_KEY>. Do not pass keys in URLs.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/heyyumi-ai-openapi.json
  type: http
- description: Alternative header auth. Query-string api_key is deprecated.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/heyyumi-ai-openapi.json
  type: apiKey
slug: heyyumi-ai-authentication
source_filename: heyyumi-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/heyyumi-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Preferred: Authorization: Bearer <API_KEY>. Do not pass keys in URLs.'\n  sources:\n  - openapi/heyyumi-ai-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Alternative header auth. Query-string api_key is deprecated.\n  sources:\n  - openapi/heyyumi-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/heyyumi-ai/authentication/heyyumi-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
---
