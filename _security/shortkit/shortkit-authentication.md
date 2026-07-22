---
api_key_in:
- header
api_specs:
- filename: shortkit-openapi.yaml
  format: yaml
  label: ShortKit API
  slug: shortkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortkit/refs/heads/main/openapi/shortkit-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shortkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShortKit secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ShortKit
provider_slug: shortkit
scheme_count: 2
schemes:
- description: Publishable key (prefix pk_{env}_). Read-only access to published content plus event ingestion and survey-response submission. Safe for client-side/mobile use.
  in: header
  name: PublishableKey
  parameter: X-API-Key
  sources:
  - openapi/shortkit-openapi.yaml
  type: apiKey
- description: Secret key (prefix sk_{env}_) sent as a Bearer token. Full management access. Server-side only; bcrypt-hashed at rest and shown once at creation.
  name: SecretKey
  scheme: bearer
  sources:
  - openapi/shortkit-openapi.yaml
  type: http
slug: shortkit-authentication
source_filename: shortkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/shortkit-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: PublishableKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Publishable key (prefix pk_{env}_). Read-only access to published content plus\n    event ingestion and survey-response submission. Safe for client-side/mobile use.\n  sources:\n  - openapi/shortkit-openapi.yaml\n- name: SecretKey\n  type: http\n  scheme: bearer\n  description: Secret key (prefix sk_{env}_) sent as a Bearer token. Full management access.\n    Server-side only; bcrypt-hashed at rest and shown once at creation.\n  sources:\n  - openapi/shortkit-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shortkit/refs/heads/main/authentication/shortkit-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Video
- Short-Form Video
- Video SDK
- Streaming
- Live Streaming
- Content Delivery
- Analytics
- Advertising
- Y Combinator
---
