---
api_key_in:
- header
api_specs:
- filename: genki-forest-open-platform-swagger.json
  format: json
  label: Genki Forest Open Platform — Distributor & Receivables Management
  slug: genki-forest-open-platform-distributor-receivables-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genki-forest/refs/heads/main/openapi/genki-forest-open-platform-swagger.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Genki Forest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genki Forest secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Genki Forest
provider_slug: genki-forest
scheme_count: 2
schemes:
- in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/genki-forest-open-platform-swagger.json
  type: apiKey
- in: header
  name: tenantNumber
  parameter: tenantNumber
  sources:
  - openapi/genki-forest-open-platform-swagger.json
  type: apiKey
slug: genki-forest-authentication
source_filename: genki-forest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: derived\nsource: openapi/genki-forest-open-platform-swagger.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/genki-forest-open-platform-swagger.json\n- name: tenantNumber\n  type: apiKey\n  in: header\n  parameter: tenantNumber\n  sources:\n  - openapi/genki-forest-open-platform-swagger.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genki-forest/refs/heads/main/authentication/genki-forest-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Beverages
- Food and Beverage
- Consumer Packaged Goods
- Manufacturing
- Distribution
- Retail
- China
---
