---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: tapeperp-com-free-api-openapi.yml
  format: yaml
  label: Tape Free API
  slug: tapeperp-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapeperp-com/openapi/tapeperp-com-free-api-openapi.yml
- filename: tapeperp-com-paid-api-openapi.yml
  format: yaml
  label: Tape Paid API
  slug: tapeperp-com-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapeperp-com/openapi/tapeperp-com-paid-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Tape Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tape secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tape
provider_slug: tapeperp-com
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/tapeperp-com-openapi.json
  type: apiKey
- in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/tapeperp-com-openapi.json
  type: apiKey
slug: tapeperp-com-authentication
source_filename: tapeperp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/tapeperp-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/tapeperp-com-openapi.json\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/tapeperp-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tapeperp-com/authentication/tapeperp-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analytics
- Cryptocurrency
- MarketData
- RealTime
- Finance
---
