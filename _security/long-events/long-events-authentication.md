---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: long-events-discovery-api-openapi.yml
  format: yaml
  label: LONG Events Discovery API
  slug: long-events-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-discovery-api-openapi.yml
- filename: long-events-event-weeks-api-openapi.yml
  format: yaml
  label: LONG Events Event weeks API
  slug: long-events-event-weeks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-event-weeks-api-openapi.yml
- filename: long-events-events-and-artists-api-openapi.yml
  format: yaml
  label: LONG Events Events and artists API
  slug: long-events-events-and-artists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-events-and-artists-api-openapi.yml
- filename: long-events-long-5-api-openapi.yml
  format: yaml
  label: LONG Events LONG 5 API
  slug: long-events-long-5-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-long-5-api-openapi.yml
- filename: long-events-mcp-api-openapi.yml
  format: yaml
  label: LONG Events MCP API
  slug: long-events-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-mcp-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: LONG Events Authentication
name_suffix: Authentication
oauth_flows: []
overview: LONG Events secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LONG Events
provider_slug: long-events
scheme_count: 4
schemes:
- description: LONG key (`long_...`) or Belong key (`sk_...`).
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/long-events-openapi.json
  type: apiKey
- description: Signed x402-v2, self-facilitated BSC stablecoin/LONG tx-hash proof, or B402 payment payload selected from a 402 response. `X-PAYMENT` is accepted as a compatibility alias.
  in: header
  name: PaymentSignature
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/long-events-openapi.json
  type: apiKey
- description: Reusable payment-session token returned after a successful bundled payment.
  in: header
  name: PaymentSession
  parameter: X-402-Token
  sources:
  - openapi/long-events-openapi.json
  type: apiKey
- description: Opt an API-key request into prepaid credit billing.
  in: header
  name: Credits
  parameter: X-Pay-With-Credits
  sources:
  - openapi/long-events-openapi.json
  type: apiKey
slug: long-events-authentication
source_filename: long-events-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/long-events-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: LONG key (`long_...`) or Belong key (`sk_...`).\n  sources:\n  - openapi/long-events-openapi.json\n- name: PaymentSignature\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Signed x402-v2, self-facilitated BSC stablecoin/LONG tx-hash proof, or B402 payment\n    payload selected from a 402 response. `X-PAYMENT` is accepted as a compatibility alias.\n  sources:\n  - openapi/long-events-openapi.json\n- name: PaymentSession\n  type: apiKey\n  in: header\n  parameter: X-402-Token\n  description: Reusable payment-session token returned after a successful bundled payment.\n  sources:\n  - openapi/long-events-openapi.json\n- name: Credits\n  type: apiKey\n  in: header\n  parameter: X-Pay-With-Credits\n  description: Opt\
  \ an API-key request into prepaid credit billing.\n  sources:\n  - openapi/long-events-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/long-events/authentication/long-events-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Event
- Artificial Intelligence
- Data
- MCP
- REST
---
