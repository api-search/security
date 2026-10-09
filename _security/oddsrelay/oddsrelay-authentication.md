---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: oddsrelay-account-api-openapi.yml
  format: yaml
  label: OddsRelay Account API
  slug: oddsrelay-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/openapi/oddsrelay-account-api-openapi.yml
- filename: oddsrelay-discovery-api-openapi.yml
  format: yaml
  label: OddsRelay Discovery API
  slug: oddsrelay-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/openapi/oddsrelay-discovery-api-openapi.yml
- filename: oddsrelay-odds-api-openapi.yml
  format: yaml
  label: OddsRelay Odds API
  slug: oddsrelay-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/openapi/oddsrelay-odds-api-openapi.yml
- filename: oddsrelay-service-api-openapi.yml
  format: yaml
  label: OddsRelay Service API
  slug: oddsrelay-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/openapi/oddsrelay-service-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Oddsrelay Authentication
name_suffix: Authentication
oauth_flows: []
overview: OddsRelay secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OddsRelay
provider_slug: oddsrelay
scheme_count: 2
schemes:
- description: '`Authorization: Bearer or_live_…`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oddsrelay-openapi.yml
  type: http
- description: The same key in `x-api-key`.
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/oddsrelay-openapi.yml
  type: apiKey
slug: oddsrelay-authentication
source_filename: oddsrelay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/oddsrelay-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: '`Authorization: Bearer or_live_…`'\n  sources:\n  - openapi/oddsrelay-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The same key in `x-api-key`.\n  sources:\n  - openapi/oddsrelay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/authentication/oddsrelay-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Sports Betting
- Odds
- Sports Data
- Matched Betting
- Data Feeds
---
