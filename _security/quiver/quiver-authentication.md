---
api_key_in: []
api_specs:
- filename: quiver-openapi.yml
  format: yaml
  label: Quiver Quantitative API
  slug: quiver
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver/refs/heads/main/openapi/quiver-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quiver Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quiver Quantitative secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quiver Quantitative
provider_slug: quiver
scheme_count: 1
schemes:
- description: 'Bearer token from your Quiver Quantitative account. Pass as `Authorization: Bearer <API_KEY>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/quiver-openapi.yml
  type: http
slug: quiver-authentication
source_filename: quiver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quiver-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token from your Quiver Quantitative account. Pass as `Authorization:\n    Bearer <API_KEY>`.'\n  sources:\n  - openapi/quiver-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quiver/refs/heads/main/authentication/quiver-authentication.yml
summary_line: http · 1 scheme
tags:
- Alternative Data
- Financial Data
- Investment Research
- Market Data
- Government Data
- Congressional Trading
---
