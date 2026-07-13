---
api_key_in: []
api_specs:
- filename: starfish-data-platform-openapi.yml
  format: yaml
  label: Itron Starfish Data Platform API
  slug: itron-starfish-data-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itron/refs/heads/main/openapi/starfish-data-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Itron Authentication
name_suffix: Authentication
oauth_flows: []
overview: Itron secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Itron
provider_slug: itron
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token issued by the Tokens API (short-lived) or obtained via OAuth client credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/starfish-data-platform-openapi.yml
  type: http
slug: itron-authentication
source_filename: itron-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/starfish-data-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token issued by the Tokens API (short-lived) or obtained via OAuth client\n    credentials.\n  sources:\n  - openapi/starfish-data-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itron/refs/heads/main/authentication/itron-authentication.yml
summary_line: http · 1 scheme
tags:
- Itron
- Utilities
- Smart Meters
- Smart Grid
- Smart Cities
- Internet Of Things
- IoT
- Energy
- Water
- Gas
- Electricity
- Distributed Intelligence
- Grid Edge
- AMI
- AMR
- RF Mesh
- IPv6
- OData
- Industrial IoT
- Fortune 1000
- NASDAQ ITRI
---
