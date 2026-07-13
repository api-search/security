---
api_key_in:
- query
api_specs:
- filename: offenders-io-openapi.yml
  format: yaml
  label: Offenders.io
  slug: offenders-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offenders-io/refs/heads/main/openapi/offenders-io-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Offenders Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Offenders.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Offenders.io
provider_slug: offenders-io
scheme_count: 1
schemes:
- in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/offenders-io-openapi.yml
  type: apiKey
slug: offenders-io-authentication
source_filename: offenders-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/offenders-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/offenders-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offenders-io/refs/heads/main/authentication/offenders-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sex Offenders
- Public Safety
- Criminal Records
---
