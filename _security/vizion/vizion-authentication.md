---
api_key_in:
- header
api_specs:
- filename: vizion-container-tracking-openapi.yml
  format: yaml
  label: Vizion Container Tracking API
  slug: container-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vizion/refs/heads/main/openapi/vizion-container-tracking-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vizion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vizion secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vizion
provider_slug: vizion
scheme_count: 1
schemes:
- description: Your Vizion API key. Include in all requests.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/vizion-container-tracking-openapi.yml
  type: apiKey
slug: vizion-authentication
source_filename: vizion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vizion-container-tracking-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your Vizion API key. Include in all requests.\n  sources:\n  - openapi/vizion-container-tracking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vizion/refs/heads/main/authentication/vizion-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Container Tracking
- Logistics
- Ocean Freight
- Shipping
- Supply Chain
- Webhooks
---
