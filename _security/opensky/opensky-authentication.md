---
api_key_in: []
api_specs:
- filename: opensky-rest-api.json
  format: json
  label: OpenSky Network REST API
  slug: opensky-network-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensky/refs/heads/main/openapi/opensky-rest-api.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opensky Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenSky Network secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenSky Network
provider_slug: opensky
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 client credentials Bearer token obtained from https://auth.opensky-network.org/auth/realms/opensky-network/protocol/openid-connect/token. Tokens expire after 30 minutes.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/opensky-rest-api.json
  type: http
slug: opensky-authentication
source_filename: opensky-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opensky-rest-api.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 client credentials Bearer token obtained from https://auth.opensky-network.org/auth/realms/opensky-network/protocol/openid-connect/token.\n    Tokens expire after 30 minutes.\n  sources:\n  - openapi/opensky-rest-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensky/refs/heads/main/authentication/opensky-authentication.yml
summary_line: http · 1 scheme
tags:
- Aviation
- Flight Tracking
- ADS-B
- Aircraft
- Airport
- Real-Time
- Historical Data
---
