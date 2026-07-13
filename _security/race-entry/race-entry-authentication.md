---
api_key_in:
- query
api_specs:
- filename: race-entry-openapi.yml
  format: yaml
  label: Race Entry
  slug: race-entry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Race Entry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Race Entry secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Race Entry
provider_slug: race-entry
scheme_count: 1
schemes:
- description: Temporary key returned from /login. Must be supplied alongside tmp_secret query parameter. Credentials expire after 48 hours.
  in: query
  name: TempCredentials
  parameter: tmp_key
  sources:
  - openapi/race-entry-openapi.yml
  type: apiKey
slug: race-entry-authentication
source_filename: race-entry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/race-entry-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: TempCredentials\n  type: apiKey\n  in: query\n  parameter: tmp_key\n  description: Temporary key returned from /login. Must be supplied alongside tmp_secret query\n    parameter. Credentials expire after 48 hours.\n  sources:\n  - openapi/race-entry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/authentication/race-entry-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Race Timing
- Race Registration
- Event Management
- Race Results
- Sports
---
