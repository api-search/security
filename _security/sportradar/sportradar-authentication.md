---
api_key_in:
- header
- query
api_specs:
- filename: sportradar-sports-data-openapi.yml
  format: yaml
  label: Sportradar Sports Data API
  slug: sports-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/openapi/sportradar-sports-data-openapi.yml
- filename: sportradar-push-feeds-openapi.yml
  format: yaml
  label: Sportradar Push Feeds API
  slug: push-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/openapi/sportradar-push-feeds-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sportradar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sportradar secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sportradar
provider_slug: sportradar
scheme_count: 2
schemes:
- description: Sportradar Push Feeds require an API key passed in the x-api-key request header. Push entitlements are tied to Realtime customer accounts.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/sportradar-push-feeds-openapi.yml
  type: apiKey
- description: Sportradar API key passed as a query parameter. Obtain from the Sportradar developer portal.
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/sportradar-sports-data-openapi.yml
  type: apiKey
slug: sportradar-authentication
source_filename: sportradar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sportradar-push-feeds-openapi.yml, openapi/sportradar-sports-data-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Sportradar Push Feeds require an API key passed in the x-api-key request header.\n    Push entitlements are tied to Realtime customer accounts.\n  sources:\n  - openapi/sportradar-push-feeds-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Sportradar API key passed as a query parameter. Obtain from the Sportradar developer\n    portal.\n  sources:\n  - openapi/sportradar-sports-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/authentication/sportradar-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data
- Esports
- Fantasy Sports
- HTTP Chunked
- Media
- Push
- Real-Time
- Sports
- Sports Data
- Statistics
- Streaming
---
