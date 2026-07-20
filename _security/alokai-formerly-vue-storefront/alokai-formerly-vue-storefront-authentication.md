---
api_key_in:
- header
api_specs:
- filename: alokai-formerly-vue-storefront-cloud-openapi.json
  format: json
  label: Alokai Cloud API
  slug: alokai-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alokai-formerly-vue-storefront/refs/heads/main/openapi/alokai-formerly-vue-storefront-cloud-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Alokai Formerly Vue Storefront Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alokai (formerly Vue Storefront) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alokai (formerly Vue Storefront)
provider_slug: alokai-formerly-vue-storefront
scheme_count: 2
schemes:
- description: API key identifying the caller, paired with X-User-Id.
  in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - https://docs.alokai.com/cloud/api/access
  type: apiKey
- description: User identifier paired with X-Api-Key to authorize Cloud API access.
  in: header
  name: UserId
  parameter: X-User-Id
  sources:
  - https://docs.alokai.com/cloud/api/access
  type: apiKey
slug: alokai-formerly-vue-storefront-authentication
source_filename: alokai-formerly-vue-storefront-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.alokai.com/cloud/api/access\ndocs: https://docs.alokai.com/cloud/api/access\nnote: >-\n  The Alokai Cloud (farmer) OpenAPI does not declare securitySchemes in-spec.\n  The auth model is documented: access is granted by a paired X-Api-Key and\n  X-User-Id request header. Captured from the docs (searched), not derived.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key identifying the caller, paired with X-User-Id.\n  sources: [https://docs.alokai.com/cloud/api/access]\n- name: UserId\n  type: apiKey\n  in: header\n  parameter: X-User-Id\n  description: User identifier paired with X-Api-Key to authorize Cloud API access.\n  sources: [https://docs.alokai.com/cloud/api/access]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alokai-formerly-vue-storefront/refs/heads/main/authentication/alokai-formerly-vue-storefront-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Saas
- Ecommerce
- Composable Commerce
- Headless Commerce
- Frontend as a Service
- Storefront
- SDK
- Middleware
- Cloud Hosting
---
