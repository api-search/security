---
api_key_in:
- header
api_specs:
- filename: cdisc-library-openapi.yml
  format: yaml
  label: CDISC Library API
  slug: cdisc-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-library-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cdisc Authentication
name_suffix: Authentication
oauth_flows: []
overview: cdisc secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: cdisc
provider_slug: cdisc
scheme_count: 1
schemes:
- description: API key obtained from CDISC Library API Management Developer Portal at https://api.developer.library.cdisc.org/
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/cdisc-library-openapi.yml
  type: apiKey
slug: cdisc-authentication
source_filename: cdisc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cdisc-library-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key obtained from CDISC Library API Management Developer Portal at https://api.developer.library.cdisc.org/\n  sources:\n  - openapi/cdisc-library-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/authentication/cdisc-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
