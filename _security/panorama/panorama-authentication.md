---
api_key_in:
- header
- query
api_specs:
- filename: panorama-openapi.yml
  format: yaml
  label: Panorama API
  slug: panorama
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panorama/refs/heads/main/openapi/panorama-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Panorama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Panorama secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Panorama
provider_slug: panorama
scheme_count: 2
schemes:
- description: API key generated via `/api/?type=keygen`.
  in: header
  name: ApiKeyHeader
  parameter: X-PAN-KEY
  sources:
  - openapi/panorama-openapi.yml
  type: apiKey
- description: API key passed as a query parameter (XML API).
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/panorama-openapi.yml
  type: apiKey
slug: panorama-authentication
source_filename: panorama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/panorama-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-PAN-KEY\n  description: API key generated via `/api/?type=keygen`.\n  sources:\n  - openapi/panorama-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key passed as a query parameter (XML API).\n  sources:\n  - openapi/panorama-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panorama/refs/heads/main/authentication/panorama-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Firewall Management
- Network Security
- Palo Alto Networks
---
