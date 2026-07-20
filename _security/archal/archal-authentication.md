---
api_key_in:
- header
api_specs:
- filename: archal-openapi-original.json
  format: json
  label: Archal API
  slug: archal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archal/refs/heads/main/openapi/archal-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Archal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Archal secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Archal
provider_slug: archal
scheme_count: 2
schemes:
- bearerFormat: Archal API token
  name: archalToken
  scheme: bearer
  sources:
  - openapi/archal-openapi-original.json
  type: http
- in: header
  name: routeAuthorization
  parameter: x-route-authorization
  sources:
  - openapi/archal-openapi-original.json
  type: apiKey
slug: archal-authentication
source_filename: archal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/archal-openapi-original.json\ndocs: https://docs.archal.ai/guides/authentication\nnotes: >\n  Control-plane calls use an Archal bearer token (user token via `archal login` or a\n  workspace API key `archal_ws_<key>` set as ARCHAL_TOKEN). The runtime clone proxy uses a\n  two-header model: `x-route-authorization` authenticates the outer route hop while the\n  service-shaped `Authorization` header is preserved for the clone to see. No OAuth scopes\n  (bearer + route apiKey only); a device-authorization grant (RFC 8628) is used for CLI login.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: archalToken\n  type: http\n  scheme: bearer\n  bearerFormat: Archal API token\n  sources:\n  - openapi/archal-openapi-original.json\n- name: routeAuthorization\n  type: apiKey\n  in: header\n  parameter: x-route-authorization\n  sources:\n  - openapi/archal-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archal/refs/heads/main/authentication/archal-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI Agents
- Agent Testing
- Developer Tools
- API Testing
- Sandbox
- Evaluation
- Infrastructure
---
