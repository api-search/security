---
api_key_in:
- query
api_specs:
- filename: gender-api-openapi.yml
  format: yaml
  label: Gender API
  slug: gender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gender-api/refs/heads/main/openapi/gender-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gender Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gender API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gender API
provider_slug: gender-api
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/gender-api-openapi.yml
  type: apiKey
slug: gender-api-authentication
source_filename: gender-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gender-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/gender-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gender-api/refs/heads/main/authentication/gender-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Demographics
- Gender
- Identity
- Names
- Personal Data
---
