---
api_key_in:
- header
api_specs:
- filename: openfigi-openapi.json
  format: json
  label: OpenFIGI API
  slug: openfigi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfigi/refs/heads/main/openapi/openfigi-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openfigi Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenFIGI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenFIGI
provider_slug: openfigi
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-OPENFIGI-APIKEY
  sources:
  - openapi/openfigi-openapi.json
  type: apiKey
slug: openfigi-authentication
source_filename: openfigi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openfigi-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-OPENFIGI-APIKEY\n  sources:\n  - openapi/openfigi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfigi/refs/heads/main/authentication/openfigi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial
- Instruments
---
