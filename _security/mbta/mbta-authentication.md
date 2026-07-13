---
api_key_in:
- header
- query
api_specs:
- filename: mbta-mbta-v3-api-openapi.yml
  format: yaml
  label: MBTA V3 API
  slug: mbta-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-mbta-v3-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mbta Authentication
name_suffix: Authentication
oauth_flows: []
overview: MBTA secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MBTA
provider_slug: mbta
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/mbta-mbta-v3-api-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/mbta-mbta-v3-api-openapi.yml
  type: apiKey
slug: mbta-authentication
source_filename: mbta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mbta-mbta-v3-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/mbta-mbta-v3-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/mbta-mbta-v3-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/authentication/mbta-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Boston
- Massachusetts
- Public Transportation
- Real-Time
- Transit
---
