---
api_key_in:
- query
api_specs:
- filename: nasdaq-omx-group-openapi.yml
  format: yaml
  label: Nasdaq Data Link Time-series API
  slug: data-link-time-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasdaq-omx-group/refs/heads/main/openapi/nasdaq-omx-group-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nasdaq Omx Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nasdaq secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nasdaq
provider_slug: nasdaq-omx-group
scheme_count: 1
schemes:
- description: Pass your Nasdaq Data Link API key as the `api_key` query parameter.
  in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/nasdaq-omx-group-openapi.yml
  type: apiKey
slug: nasdaq-omx-group-authentication
source_filename: nasdaq-omx-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nasdaq-omx-group-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Pass your Nasdaq Data Link API key as the `api_key` query parameter.\n  sources:\n  - openapi/nasdaq-omx-group-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-omx-group/refs/heads/main/authentication/nasdaq-omx-group-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial Services
- Capital Markets
- Stock Exchange
- Market Data
- Economics
- Fortune 1000
---
