---
api_key_in:
- header
api_specs:
- filename: helika-events-openapi.json
  format: json
  label: Helika Analytics Service
  slug: helika-analytics-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helika/refs/heads/main/openapi/helika-events-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Helika Authentication
name_suffix: Authentication
oauth_flows: []
overview: Helika secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Helika
provider_slug: helika
scheme_count: 1
schemes:
- description: API key issued from the Helika platform (platform.helika.io), sent on every request as the x-api-key header. The SDKs support both DEV and PROD keys.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  required: true
  sources:
  - https://docs.helika.io/reference/create_event_v1_events_post
  type: apiKey
slug: helika-authentication
source_filename: helika-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.helika.io/reference/create_event_v1_events_post\ndocs: https://docs.helika.io/docs/getting-started\nnote: >-\n  The published OpenAPI (openapi/helika-events-openapi.json) does not declare a\n  components.securitySchemes object; the API key is modeled as a required\n  x-api-key request header. This profile is captured from the Helika API\n  reference documentation, which documents x-api-key header authentication.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  required: true\n  description: >-\n    API key issued from the Helika platform (platform.helika.io), sent on every\n    request as the x-api-key header. The SDKs support both DEV and PROD keys.\n  sources:\n  - https://docs.helika.io/reference/create_event_v1_events_post\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helika/refs/heads/main/authentication/helika-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Gaming
- Analytics
- Game Analytics
- Web3
- Events
- AI
- SDK
- Player Data
---
