---
api_key_in:
- header
api_specs:
- filename: renesas-web-data-openapi-original.yml
  format: yaml
  label: Renesas Web Data API
  slug: renesas-web-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/openapi/renesas-web-data-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Renesas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Renesas secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Renesas
provider_slug: renesas
scheme_count: 1
schemes:
- description: 'API key passed in the x-api-key request header on every call, e.g. `x-api-key: YOUR_API_KEY`. Also send `Accept: application/json`.'
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/renesas-web-data-openapi-original.yml
  type: apiKey
slug: renesas-authentication
source_filename: renesas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/renesas-web-data-openapi-original.yml\ndocs: https://developer.renesas.com/docs/web-data-api/guides/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\naccess_model: >-\n  API key authentication. Keys are issued to approved partners and integrators\n  only, via the Web Data API access-request form; there is no self-service\n  signup. The key is used by Renesas to identify/authorize the application,\n  track usage, apply per-key rate limits, and scope which endpoints and data the\n  caller may access.\naccess_request: https://www.renesas.com/en/form/web-data-api-access-request\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    API key passed in the x-api-key request header on every call, e.g.\n    `x-api-key: YOUR_API_KEY`. Also send `Accept: application/json`.\n  sources:\n  - openapi/renesas-web-data-openapi-original.yml\nnotes:\n- The\
  \ Redocly-generated MCP server and its OAuth 2.0 authorization-server\n  metadata (well-known/renesas-oauth-authorization-server.json) govern the docs\n  MCP endpoint only; the Web Data API itself is authenticated solely by the\n  x-api-key header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/authentication/renesas-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Semiconductors
- Microcontrollers
- Electronics
- Hardware
- Product Data
- Developer Portal
- Automotive
- Industrial
- Embedded
---
