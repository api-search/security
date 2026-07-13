---
api_key_in: []
api_specs:
- filename: reloadly-gift-cards-openapi.yml
  format: yaml
  label: Reloadly Gift Cards API
  slug: gift-cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-gift-cards-openapi.yml
- filename: reloadly-airtime-openapi.yml
  format: yaml
  label: Reloadly Airtime API
  slug: airtime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-airtime-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reloadly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reloadly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reloadly
provider_slug: reloadly
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained via the /oauth/token endpoint using client credentials grant.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/reloadly-airtime-openapi.yml
  - openapi/reloadly-gift-cards-openapi.yml
  type: http
slug: reloadly-authentication
source_filename: reloadly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reloadly-airtime-openapi.yml, openapi/reloadly-gift-cards-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained via the /oauth/token endpoint using client credentials\n    grant.\n  sources:\n  - openapi/reloadly-airtime-openapi.yml\n  - openapi/reloadly-gift-cards-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/authentication/reloadly-authentication.yml
summary_line: http · 1 scheme
tags:
- Gift Cards
- Payments
- Airtime
- Mobile Top-Up
- Rewards
- Incentives
---
