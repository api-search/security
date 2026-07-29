---
api_key_in: []
api_specs:
- filename: buywhere-openapi.yml
  format: yaml
  label: BuyWhere Product Catalog API
  slug: product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buywhere/refs/heads/main/openapi/buywhere-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Buywhere Authentication
name_suffix: Authentication
oauth_flows: []
overview: BuyWhere secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BuyWhere
provider_slug: buywhere
scheme_count: 1
schemes:
- description: 'Pass your API key as a Bearer token. Get a free key at `POST /v1/auth/register`.

    Tiers: `bw_free_*` (60 rpm), `bw_live_*` (600 rpm), `bw_partner_*` (unlimited).'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/buywhere-openapi.yml
  type: http
slug: buywhere-authentication
source_filename: buywhere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/buywhere-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Pass your API key as a Bearer token. Get a free key at `POST /v1/auth/register`.\n    Tiers: `bw_free_*` (60 rpm), `bw_live_*` (600 rpm), `bw_partner_*` (unlimited).\n  sources:\n  - openapi/buywhere-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buywhere/refs/heads/main/authentication/buywhere-authentication.yml
summary_line: http · 1 scheme
tags:
- E-commerce
- Shopping
- Price Comparison
- SEA
- Southeast Asia
- AI Agents
- Product Catalog
---
