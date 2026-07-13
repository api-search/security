---
api_key_in:
- header
api_specs:
- filename: spothero-parking-openapi.yml
  format: yaml
  label: SpotHero Parking API
  slug: spothero-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spothero/refs/heads/main/openapi/spothero-parking-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spothero Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpotHero secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpotHero
provider_slug: spothero
scheme_count: 1
schemes:
- description: Partner API key issued by SpotHero
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/spothero-parking-openapi.yml
  type: apiKey
slug: spothero-authentication
source_filename: spothero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spothero-parking-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Partner API key issued by SpotHero\n  sources:\n  - openapi/spothero-parking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spothero/refs/heads/main/authentication/spothero-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Parking
- Mobility
- Transportation
- Navigation
- Reservations
---
