---
api_key_in: []
api_specs:
- filename: albertsons-audiences-api-openapi.yml
  format: yaml
  label: albertsons Audiences API
  slug: albertsons-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/openapi/albertsons-audiences-api-openapi.yml
- filename: albertsons-campaigns-api-openapi.yml
  format: yaml
  label: albertsons Campaigns API
  slug: albertsons-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/openapi/albertsons-campaigns-api-openapi.yml
- filename: albertsons-performance-api-openapi.yml
  format: yaml
  label: albertsons Performance API
  slug: albertsons-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/openapi/albertsons-performance-api-openapi.yml
- filename: albertsons-reporting-api-openapi.yml
  format: yaml
  label: albertsons Reporting API
  slug: albertsons-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/openapi/albertsons-reporting-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Albertsons Authentication
name_suffix: Authentication
oauth_flows: []
overview: albertsons secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: albertsons
provider_slug: albertsons
scheme_count: 1
schemes:
- description: Bearer token authentication via Azure AD OAuth2.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/albertsons-audiences-api-openapi.yml
  - openapi/albertsons-campaigns-api-openapi.yml
  - openapi/albertsons-performance-api-openapi.yml
  - openapi/albertsons-reporting-api-openapi.yml
  type: http
slug: albertsons-authentication
source_filename: albertsons-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/albertsons-audiences-api-openapi.yml, openapi/albertsons-campaigns-api-openapi.yml,\n  openapi/albertsons-performance-api-openapi.yml, openapi/albertsons-reporting-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication via Azure AD OAuth2.\n  sources:\n  - openapi/albertsons-audiences-api-openapi.yml\n  - openapi/albertsons-campaigns-api-openapi.yml\n  - openapi/albertsons-performance-api-openapi.yml\n  - openapi/albertsons-reporting-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/authentication/albertsons-authentication.yml
summary_line: http · 1 scheme
tags:
- Grocery
- Retail
- Retail Media
- Advertising
- Campaigns
- Analytics
- Consumer Goods
- Food
- Pharmacy
---
