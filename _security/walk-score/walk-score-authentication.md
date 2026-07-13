---
api_key_in:
- query
api_specs:
- filename: walk-score-openapi.yml
  format: yaml
  label: Walk Score API
  slug: walk-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walk-score/refs/heads/main/openapi/walk-score-openapi.yml
- filename: walk-score-transit-openapi.yml
  format: yaml
  label: Walk Score Transit API
  slug: walk-score-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walk-score/refs/heads/main/openapi/walk-score-transit-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Walk Score Authentication
name_suffix: Authentication
oauth_flows: []
overview: Walk Score secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Walk Score
provider_slug: walk-score
scheme_count: 1
schemes:
- description: Walk Score API key, contact Walk Score to obtain
  in: query
  name: apiKey
  parameter: wsapikey
  sources:
  - openapi/walk-score-openapi.yml
  - openapi/walk-score-transit-openapi.yml
  type: apiKey
slug: walk-score-authentication
source_filename: walk-score-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/walk-score-openapi.yml, openapi/walk-score-transit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: wsapikey\n  description: Walk Score API key, contact Walk Score to obtain\n  sources:\n  - openapi/walk-score-openapi.yml\n  - openapi/walk-score-transit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walk-score/refs/heads/main/authentication/walk-score-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Walkability
- Transit
- Bikeability
- Location
- Real Estate
- Urban Planning
- Transportation
---
