---
api_key_in:
- header
api_specs:
- filename: freedom-of-information-act-openapi.yml
  format: yaml
  label: Freedom of Information Act (FOIA) API
  slug: freedom-of-information-act-foia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freedom-of-information-act/refs/heads/main/openapi/freedom-of-information-act-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Freedom Of Information Act Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freedom of Information Act secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Freedom of Information Act
provider_slug: freedom-of-information-act
scheme_count: 2
schemes:
- description: API key for FOIA.gov public APIs.
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/freedom-of-information-act-openapi.yml
  type: apiKey
- description: Shared secret token between Portal and agency.
  in: header
  name: SharedSecret
  parameter: FOIA-API-SECRET
  sources:
  - openapi/freedom-of-information-act-openapi.yml
  type: apiKey
slug: freedom-of-information-act-authentication
source_filename: freedom-of-information-act-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freedom-of-information-act-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for FOIA.gov public APIs.\n  sources:\n  - openapi/freedom-of-information-act-openapi.yml\n- name: SharedSecret\n  type: apiKey\n  in: header\n  parameter: FOIA-API-SECRET\n  description: Shared secret token between Portal and agency.\n  sources:\n  - openapi/freedom-of-information-act-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freedom-of-information-act/refs/heads/main/authentication/freedom-of-information-act-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- FOIA
- Transparency
---
