---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: lots-link-lotslink-api-openapi.yml
  format: yaml
  label: LotsLink Lots Link API
  slug: lots-link-lotslink-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lots-link/openapi/lots-link-lotslink-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LotsLink Authentication
name_suffix: Authentication
oauth_flows: []
overview: LotsLink secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LotsLink
provider_slug: lots-link
scheme_count: 1
schemes:
- description: 'API key for authentication. Format: REDACTED_STRIPE_KEY'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/lots-link-openapi.json
  type: apiKey
slug: lots-link-authentication
source_filename: lots-link-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lots-link-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key for authentication. Format: REDACTED_STRIPE_KEY'\n  sources:\n  - openapi/lots-link-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lots-link/authentication/lots-link-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- URL Shorteners
- QR Codes
- Analytics
- AI Agents
---
