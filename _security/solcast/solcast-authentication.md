---
api_key_in: []
api_specs:
- filename: solcast-openapi.yml
  format: yaml
  label: Solcast API
  slug: solcast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solcast/refs/heads/main/openapi/solcast-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Solcast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solcast secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Solcast
provider_slug: solcast
scheme_count: 1
schemes:
- description: 'Authenticate using your Solcast API key as a Bearer token in the Authorization header: `Authorization: Bearer {api_key}`. Obtain an API key at https://toolkit.solcast.com.au/register.'
  name: apiKeyAuth
  scheme: bearer
  sources:
  - openapi/solcast-openapi.yml
  type: http
slug: solcast-authentication
source_filename: solcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/solcast-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate using your Solcast API key as a Bearer token in the Authorization\n    header: `Authorization: Bearer {api_key}`. Obtain an API key at https://toolkit.solcast.com.au/register.'\n  sources:\n  - openapi/solcast-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solcast/refs/heads/main/authentication/solcast-authentication.yml
summary_line: http · 1 scheme
tags:
- Solar
- Energy
- Forecasting
- Irradiance
- Weather
- Renewable Energy
- PV Power
---
