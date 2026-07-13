---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: GovInfo API
  slug: govinfo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Govinfo Authentication
name_suffix: Authentication
oauth_flows: []
overview: GovInfo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GovInfo
provider_slug: govinfo
scheme_count: 1
schemes:
- in: query
  name: apiKeyScheme
  parameter: api_key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: govinfo-authentication
source_filename: govinfo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyScheme\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/authentication/govinfo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Government Publishing
- Documents
- Open Data
---
