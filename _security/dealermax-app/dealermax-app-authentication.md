---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dealermax-app-dealerpublicapi-api-openapi.yml
  format: yaml
  label: DealerMAX Dealer Public API
  slug: dealermax-app-dealerpublicapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealermax-app/openapi/dealermax-app-dealerpublicapi-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Dealermax App Authentication
name_suffix: Authentication
oauth_flows: []
overview: DealerMAX secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DealerMAX
provider_slug: dealermax-app
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/dealermax-app-openapi.json
  type: apiKey
- bearerFormat: API key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dealermax-app-openapi.json
  type: http
slug: dealermax-app-authentication
source_filename: dealermax-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/dealermax-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/dealermax-app-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/dealermax-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dealermax-app/authentication/dealermax-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Dealer Identity
- AI Visibility
- CRM
---
