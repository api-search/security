---
api_key_in: []
api_specs:
- filename: cloverly-estimates-api-openapi.yml
  format: yaml
  label: Cloverly Estimates API
  slug: cloverly-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-estimates-api-openapi.yml
- filename: cloverly-purchases-api-openapi.yml
  format: yaml
  label: Cloverly Purchases API
  slug: cloverly-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-purchases-api-openapi.yml
- filename: cloverly-offset-types-api-openapi.yml
  format: yaml
  label: Cloverly Offset Types API
  slug: cloverly-offset-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-offset-types-api-openapi.yml
- filename: cloverly-account-api-openapi.yml
  format: yaml
  label: Cloverly Account API
  slug: cloverly-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-account-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloverly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloverly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloverly
provider_slug: cloverly
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cloverly-account-api-openapi.yml
  - openapi/cloverly-estimates-api-openapi.yml
  - openapi/cloverly-offset-types-api-openapi.yml
  - openapi/cloverly-purchases-api-openapi.yml
  type: http
slug: cloverly-authentication
source_filename: cloverly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloverly-account-api-openapi.yml, openapi/cloverly-estimates-api-openapi.yml,\n  openapi/cloverly-offset-types-api-openapi.yml, openapi/cloverly-purchases-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cloverly-account-api-openapi.yml\n  - openapi/cloverly-estimates-api-openapi.yml\n  - openapi/cloverly-offset-types-api-openapi.yml\n  - openapi/cloverly-purchases-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/authentication/cloverly-authentication.yml
summary_line: http · 1 scheme
tags:
- Carbon
- Carbon Credits
- Carbon Offsets
- Catalyst
- Climate
- Climate Action
- Climate Impact X
- CIX
- Decarbonization
- ESG
- Greenhouse Gas
- Net Zero
- Project Developers
- Registries
- Sustainability
- Voluntary Carbon Market
- VCM
---
