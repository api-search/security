---
api_key_in:
- header
- query
api_specs:
- filename: what3words-openapi.yml
  format: yaml
  label: what3words Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/what3words/refs/heads/main/openapi/what3words-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: What3Words Authentication
name_suffix: Authentication
oauth_flows: []
overview: what3words secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: what3words
provider_slug: what3words
scheme_count: 2
schemes:
- in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/what3words-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/what3words-openapi.yml
  type: apiKey
slug: what3words-authentication
source_filename: what3words-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/what3words-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/what3words-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/what3words-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/what3words/refs/heads/main/authentication/what3words-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Geocoding
- Addressing
- Location
- Three Word Address
- Maps
---
