---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lead-radar-fr-api-openapi.json
  format: json
  label: Lead Radar API API
  slug: lead-radar-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lead-radar-fr/openapi/_original/lead-radar-fr-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lead Radar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lead Radar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lead Radar
provider_slug: lead-radar-fr
scheme_count: 1
schemes:
- description: 'API key (lr_...) from POST /api/auth/register with createApiKey: true, from the dashboard settings, or issued via OAuth 2.1 (see /.well-known/oauth-authorization-server). 120 requests/minute per key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lead-radar-fr-openapi.json
  type: http
slug: lead-radar-fr-authentication
source_filename: lead-radar-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lead-radar-fr-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key (lr_...) from POST /api/auth/register with createApiKey: true, from\n    the dashboard settings, or issued via OAuth 2.1 (see /.well-known/oauth-authorization-server).\n    120 requests/minute per key.'\n  sources:\n  - openapi/lead-radar-fr-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lead-radar-fr/authentication/lead-radar-fr-authentication.yml
summary_line: http · 1 scheme
tags:
- B2B
- Lead Generation
- French Market
- Software-as-a-Service
- Prospecting
---
