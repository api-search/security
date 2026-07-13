---
api_key_in: []
api_specs:
- filename: procter-and-gamble-api-marketplace-openapi.yml
  format: yaml
  label: Procter & Gamble API Marketplace
  slug: api-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procter-and-gamble/refs/heads/main/openapi/procter-and-gamble-api-marketplace-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Procter And Gamble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Procter & Gamble secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Procter & Gamble
provider_slug: procter-and-gamble
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/procter-and-gamble-api-marketplace-openapi.yml
  type: http
slug: procter-and-gamble-authentication
source_filename: procter-and-gamble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/procter-and-gamble-api-marketplace-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/procter-and-gamble-api-marketplace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procter-and-gamble/refs/heads/main/authentication/procter-and-gamble-authentication.yml
summary_line: http · 1 scheme
tags:
- Consumer Goods
- Manufacturing
- Retail
- Supply Chain
- Fortune 100
---
