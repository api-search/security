---
api_key_in:
- query
api_specs:
- filename: open-fec-openapi.yml
  format: yaml
  label: OpenFEC API
  slug: openfec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Open Fec Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenFEC secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenFEC
provider_slug: open-fec
scheme_count: 1
schemes:
- description: api.data.gov API key. Use DEMO_KEY for limited testing.
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/open-fec-openapi.yml
  type: apiKey
slug: open-fec-authentication
source_filename: open-fec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/open-fec-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: api.data.gov API key. Use DEMO_KEY for limited testing.\n  sources:\n  - openapi/open-fec-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/authentication/open-fec-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Campaign Finance
- Elections
- FEC
- Federal
- Government
---
