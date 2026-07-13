---
api_key_in: []
api_specs:
- filename: cbre-cbre-api-openapi.yml
  format: yaml
  label: CBRE Developer API
  slug: cbre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cbre/refs/heads/main/openapi/cbre-cbre-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cbre Authentication
name_suffix: Authentication
oauth_flows: []
overview: CBRE secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CBRE
provider_slug: cbre
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cbre-cbre-api-openapi.yml
  type: http
slug: cbre-authentication
source_filename: cbre-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cbre-cbre-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cbre-cbre-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cbre/refs/heads/main/authentication/cbre-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Commercial Real Estate
- Facilities Management
- Fortune 500
- Investment Management
- Property Management
- Real Estate
- Valuation
---
