---
api_key_in:
- header
api_specs:
- filename: luxury-presence-cms-openapi.json
  format: json
  label: Luxury Presence Public API
  slug: luxury-presence-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luxury-presence/refs/heads/main/openapi/luxury-presence-cms-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Luxury Presence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luxury Presence secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Luxury Presence
provider_slug: luxury-presence
scheme_count: 1
schemes:
- description: API key generated from the Luxury Presence dashboard (Settings > API Keys). Sent as the x-api-key request header.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/luxury-presence-cms-openapi.json
  type: apiKey
slug: luxury-presence-authentication
source_filename: luxury-presence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/luxury-presence-cms-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key generated from the Luxury Presence dashboard (Settings > API Keys). Sent\n    as the x-api-key request header.\n  sources:\n  - openapi/luxury-presence-cms-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luxury-presence/refs/heads/main/authentication/luxury-presence-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Vertical Software
- Real Estate
- PropTech
- CRM
- Marketing
- Websites
- Webhooks
- Lead Generation
---
