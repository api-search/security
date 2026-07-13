---
api_key_in:
- header
api_specs:
- filename: sex-offenders-api-openapi.yml
  format: yaml
  label: Sex Offenders API
  slug: sex-offenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sex-offenders-api/refs/heads/main/openapi/sex-offenders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sex Offenders Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sex Offenders API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sex Offenders API
provider_slug: sex-offenders-api
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/sex-offenders-api-openapi.yml
  type: apiKey
slug: sex-offenders-api-authentication
source_filename: sex-offenders-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sex-offenders-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/sex-offenders-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sex-offenders-api/refs/heads/main/authentication/sex-offenders-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sex Offenders
---
