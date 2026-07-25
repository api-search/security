---
api_key_in:
- header
api_specs:
- filename: interos-groups-api-openapi.yml
  format: yaml
  label: Interos Groups API
  slug: interos-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-groups-api-openapi.yml
- filename: interos-health-api-openapi.yml
  format: yaml
  label: Interos health API
  slug: interos-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-health-api-openapi.yml
- filename: interos-organizations-api-openapi.yml
  format: yaml
  label: Interos Organizations API
  slug: interos-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-organizations-api-openapi.yml
- filename: interos-relationships-api-openapi.yml
  format: yaml
  label: Interos Relationships API
  slug: interos-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-relationships-api-openapi.yml
- filename: interos-watchtower-api-openapi.yml
  format: yaml
  label: Interos Watchtower API
  slug: interos-watchtower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-watchtower-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Interos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Interos secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Interos
provider_slug: interos
scheme_count: 2
schemes:
- in: header
  name: Interos API Key
  parameter: x-api-key
  sources:
  - openapi/interos-openapi.json
  type: apiKey
- in: header
  name: Interos Customer ID
  parameter: x-customer-id
  sources:
  - openapi/interos-openapi.json
  type: apiKey
slug: interos-authentication
source_filename: interos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/interos-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Interos API Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/interos-openapi.json\n- name: Interos Customer ID\n  type: apiKey\n  in: header\n  parameter: x-customer-id\n  sources:\n  - openapi/interos-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/authentication/interos-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Enterprise
- Supply Chain
- Risk Management
- Supplier Risk
- Third-Party Risk
- Artificial Intelligence
- API
---
