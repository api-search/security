---
api_key_in:
- header
api_specs:
- filename: meddra-terminology-openapi.yml
  format: yaml
  label: MedDRA / WHO Drug Dictionary API
  slug: meddra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-terminology-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Meddra Authentication
name_suffix: Authentication
oauth_flows: []
overview: meddra secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: meddra
provider_slug: meddra
scheme_count: 2
schemes:
- in: header
  name: APIKey
  parameter: X-API-Key
  sources:
  - openapi/meddra-terminology-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/meddra-terminology-openapi.yml
  type: http
slug: meddra-authentication
source_filename: meddra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meddra-terminology-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/meddra-terminology-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/meddra-terminology-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/authentication/meddra-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
