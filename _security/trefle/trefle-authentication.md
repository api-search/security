---
api_key_in:
- query
api_specs:
- filename: trefle-openapi.yml
  format: yaml
  label: Trefle API
  slug: trefle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trefle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trefle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trefle
provider_slug: trefle
scheme_count: 1
schemes:
- description: 'Trefle personal access token obtained by registering at trefle.io. Can be passed as a query parameter (?token=YOUR_TOKEN) or in the Authorization header (Authorization: Bearer [example key]).'
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/trefle-openapi.yml
  type: apiKey
slug: trefle-authentication
source_filename: trefle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trefle-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: 'Trefle personal access token obtained by registering at trefle.io. Can be passed\n    as a query parameter (?token=YOUR_TOKEN) or in the Authorization header (Authorization:\n    Bearer [example key]).'\n  sources:\n  - openapi/trefle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/authentication/trefle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agriculture
- Botany
- Open Data
- Plants
- Science
---
