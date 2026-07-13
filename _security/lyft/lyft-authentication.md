---
api_key_in:
- header
api_specs:
- filename: lyft-ride-sharing-openapi.yml
  format: yaml
  label: Lyft Ride-Sharing API
  slug: ride-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-ride-sharing-openapi.yml
- filename: lyft-concierge-openapi.yml
  format: yaml
  label: Lyft Concierge API
  slug: concierge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-concierge-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lyft Authentication
name_suffix: Authentication
oauth_flows: []
overview: lyft secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: lyft
provider_slug: lyft
scheme_count: 2
schemes:
- description: OAuth 2.0 access token obtained through the client credentials flow for the organization's concierge API client.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lyft-concierge-openapi.yml
  - openapi/lyft-ride-sharing-openapi.yml
  type: http
- description: Client token for accessing public endpoints without user authorization. Passed as a Bearer token in the Authorization header.
  in: header
  name: clientToken
  parameter: Authorization
  sources:
  - openapi/lyft-ride-sharing-openapi.yml
  type: apiKey
slug: lyft-authentication
source_filename: lyft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lyft-concierge-openapi.yml, openapi/lyft-ride-sharing-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token obtained through the client credentials flow for the organization's\n    concierge API client.\n  sources:\n  - openapi/lyft-concierge-openapi.yml\n  - openapi/lyft-ride-sharing-openapi.yml\n- name: clientToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Client token for accessing public endpoints without user authorization. Passed\n    as a Bearer token in the Authorization header.\n  sources:\n  - openapi/lyft-ride-sharing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/authentication/lyft-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
