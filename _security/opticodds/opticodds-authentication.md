---
api_key_in:
- header
- query
api_specs:
- filename: opticodds-openapi.yml
  format: yaml
  label: OpticOdds
  slug: opticodds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opticodds/refs/heads/main/openapi/opticodds-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opticodds Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpticOdds secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpticOdds
provider_slug: opticodds
scheme_count: 2
schemes:
- description: OpticOdds API key supplied in the X-Api-Key header.
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/opticodds-openapi.yml
  type: apiKey
- description: OpticOdds API key supplied via the `key` query parameter.
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/opticodds-openapi.yml
  type: apiKey
slug: opticodds-authentication
source_filename: opticodds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opticodds-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: OpticOdds API key supplied in the X-Api-Key header.\n  sources:\n  - openapi/opticodds-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: OpticOdds API key supplied via the `key` query parameter.\n  sources:\n  - openapi/opticodds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opticodds/refs/heads/main/authentication/opticodds-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Odds
- Sports Betting
- Sports Data
---
