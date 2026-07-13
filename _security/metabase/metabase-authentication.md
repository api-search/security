---
api_key_in:
- header
api_specs:
- filename: metabase-openapi.yml
  format: yaml
  label: Metabase API
  slug: metabase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Metabase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metabase secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Metabase
provider_slug: metabase
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/metabase-openapi.yml
  type: apiKey
- in: header
  name: SessionAuth
  parameter: X-Metabase-Session
  sources:
  - openapi/metabase-openapi.yml
  type: apiKey
slug: metabase-authentication
source_filename: metabase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metabase-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/metabase-openapi.yml\n- name: SessionAuth\n  type: apiKey\n  in: header\n  parameter: X-Metabase-Session\n  sources:\n  - openapi/metabase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/authentication/metabase-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Open Source
- SQL
---
