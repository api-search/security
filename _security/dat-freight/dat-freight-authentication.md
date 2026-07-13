---
api_key_in: []
api_specs:
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT Identity & Token API
  slug: dat-freight-identity-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT Load Board Search API
  slug: dat-freight-load-board-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT Freight Posting API
  slug: dat-freight-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT RateView Rate Lookup API
  slug: dat-freight-rateview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT BookNow API
  slug: dat-freight-booknow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT Tracking API
  slug: dat-freight-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dat Freight Authentication
name_suffix: Authentication
oauth_flows: []
overview: DAT Freight & Analytics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DAT Freight & Analytics
provider_slug: dat-freight
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: User access token obtained from POST /access/v1/token/user, which itself requires an organization token from POST /access/v1/token/organization.
  name: userToken
  scheme: bearer
  sources:
  - openapi/dat-freight-openapi.yml
  type: http
slug: dat-freight-authentication
source_filename: dat-freight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dat-freight-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: userToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: User access token obtained from POST /access/v1/token/user, which itself requires\n    an organization token from POST /access/v1/token/organization.\n  sources:\n  - openapi/dat-freight-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/authentication/dat-freight-authentication.yml
summary_line: http · 1 scheme
tags:
- Freight
- Trucking
- Load Board
- Logistics
- Freight Rates
- RateView
- Supply Chain
- Transportation
- Analytics
---
