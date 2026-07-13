---
api_key_in:
- header
api_specs:
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Betting API
  slug: betfair-betting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Accounts API
  slug: betfair-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Heartbeat API
  slug: betfair-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-asyncapi.yml
  format: yaml
  label: Betfair Exchange Stream API
  slug: betfair-exchange-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/asyncapi/betfair-asyncapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Historic Data API
  slug: betfair-historic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Betfair Authentication
name_suffix: Authentication
oauth_flows: []
overview: Betfair secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Betfair
provider_slug: betfair
scheme_count: 2
schemes:
- description: The developer Application Key (delayed or live).
  in: header
  name: appKey
  parameter: X-Application
  sources:
  - openapi/betfair-openapi.yml
  type: apiKey
- description: The session token (ssoid) obtained from identity SSO login.
  in: header
  name: sessionToken
  parameter: X-Authentication
  sources:
  - openapi/betfair-openapi.yml
  type: apiKey
slug: betfair-authentication
source_filename: betfair-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/betfair-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: appKey\n  type: apiKey\n  in: header\n  parameter: X-Application\n  description: The developer Application Key (delayed or live).\n  sources:\n  - openapi/betfair-openapi.yml\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: X-Authentication\n  description: The session token (ssoid) obtained from identity SSO login.\n  sources:\n  - openapi/betfair-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/authentication/betfair-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Betting Exchange
- Sports Betting
- Wagering
- Trading
- Market Data
- JSON-RPC
- Streaming
---
