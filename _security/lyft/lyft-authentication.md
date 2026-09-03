---
api_key_in:
- header
api_specs:
- filename: lyft-concierge-rides-api-openapi.yml
  format: yaml
  label: lyft Concierge Rides API
  slug: lyft-concierge-rides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-concierge-rides-api-openapi.yml
- filename: lyft-cost-estimates-api-openapi.yml
  format: yaml
  label: lyft Cost Estimates API
  slug: lyft-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-cost-estimates-api-openapi.yml
- filename: lyft-drivers-api-openapi.yml
  format: yaml
  label: lyft Drivers API
  slug: lyft-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-drivers-api-openapi.yml
- filename: lyft-eta-api-openapi.yml
  format: yaml
  label: lyft ETA API
  slug: lyft-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-eta-api-openapi.yml
- filename: lyft-profile-api-openapi.yml
  format: yaml
  label: lyft Profile API
  slug: lyft-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-profile-api-openapi.yml
- filename: lyft-ride-types-api-openapi.yml
  format: yaml
  label: lyft Ride Types API
  slug: lyft-ride-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-ride-types-api-openapi.yml
- filename: lyft-rides-api-openapi.yml
  format: yaml
  label: lyft Rides API
  slug: lyft-rides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-rides-api-openapi.yml
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
overview: Lyft secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lyft
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
