---
api_key_in:
- header
api_specs:
- filename: triple-whale-openapi.yml
  format: yaml
  label: Triple Whale Summary API
  slug: triple-whale-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-openapi.yml
- filename: triple-whale-openapi.yml
  format: yaml
  label: Triple Whale Attribution API
  slug: triple-whale-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-openapi.yml
- filename: triple-whale-openapi.yml
  format: yaml
  label: Triple Whale Data-In API
  slug: triple-whale-data-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Triple Whale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Triple Whale secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Triple Whale
provider_slug: triple-whale
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/triple-whale-openapi.yml
  type: apiKey
slug: triple-whale-authentication
source_filename: triple-whale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/triple-whale-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/triple-whale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/authentication/triple-whale-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-commerce
- Analytics
- Attribution
- Shopify
- Pixel Tracking
- ROAS
- DTC
- Marketing
---
