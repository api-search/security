---
api_key_in:
- query
api_specs:
- filename: perenual-perenual-openapi.yml
  format: yaml
  label: Perenual API
  slug: perenual
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perenual/refs/heads/main/openapi/perenual-perenual-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Perenual Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perenual secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Perenual
provider_slug: perenual
scheme_count: 1
schemes:
- in: query
  name: apiKeyAuth
  parameter: key
  sources:
  - openapi/perenual-perenual-openapi.yml
  type: apiKey
slug: perenual-authentication
source_filename: perenual-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/perenual-perenual-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/perenual-perenual-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perenual/refs/heads/main/authentication/perenual-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Plants
- Botany
- Gardening
- Horticulture
---
