---
api_key_in:
- header
api_specs:
- filename: openfigi-openapi.yml
  format: yaml
  label: OpenFIGI API
  slug: openfigi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-lp/refs/heads/main/openapi/openfigi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bloomberg Lp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloomberg L.P. secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bloomberg L.P.
provider_slug: bloomberg-lp
scheme_count: 1
schemes:
- description: 'Optional OpenFIGI API key. Sign up at https://www.openfigi.com/user/signup

    to receive a key and unlock higher rate limits.'
  in: header
  name: ApiKeyAuth
  parameter: X-OPENFIGI-APIKEY
  sources:
  - openapi/openfigi-openapi.yml
  type: apiKey
slug: bloomberg-lp-authentication
source_filename: bloomberg-lp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openfigi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-OPENFIGI-APIKEY\n  description: |-\n    Optional OpenFIGI API key. Sign up at https://www.openfigi.com/user/signup\n    to receive a key and unlock higher rate limits.\n  sources:\n  - openapi/openfigi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-lp/refs/heads/main/authentication/bloomberg-lp-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial Services
- Market Data
- News
- Reference Data
- Symbology
- Terminal
---
