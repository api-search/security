---
api_key_in:
- header
api_specs:
- filename: capital-com-public-api-capital-com-rest-api-openapi.yml
  format: yaml
  label: Capital.com REST API
  slug: capital-com-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capital-com-public-api/refs/heads/main/openapi/capital-com-public-api-capital-com-rest-api-openapi.yml
- filename: capital-com-public-api-asyncapi.yml
  format: yaml
  label: Capital.com WebSocket API
  slug: capital-com-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/capital-com-public-api/refs/heads/main/asyncapi/capital-com-public-api-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Capital Com Public Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capital.com Public API secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Capital.com Public API
provider_slug: capital-com-public-api
scheme_count: 3
schemes:
- description: Capital.com API key required for all calls.
  in: header
  name: apiKey
  parameter: X-CAP-API-KEY
  sources:
  - openapi/capital-com-public-api-capital-com-rest-api-openapi.yml
  type: apiKey
- description: Client session token returned after creating a session.
  in: header
  name: sessionToken
  parameter: CST
  sources:
  - openapi/capital-com-public-api-capital-com-rest-api-openapi.yml
  type: apiKey
- description: Security token returned after creating a session.
  in: header
  name: securityToken
  parameter: X-SECURITY-TOKEN
  sources:
  - openapi/capital-com-public-api-capital-com-rest-api-openapi.yml
  type: apiKey
slug: capital-com-public-api-authentication
source_filename: capital-com-public-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/capital-com-public-api-capital-com-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-CAP-API-KEY\n  description: Capital.com API key required for all calls.\n  sources:\n  - openapi/capital-com-public-api-capital-com-rest-api-openapi.yml\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: CST\n  description: Client session token returned after creating a session.\n  sources:\n  - openapi/capital-com-public-api-capital-com-rest-api-openapi.yml\n- name: securityToken\n  type: apiKey\n  in: header\n  parameter: X-SECURITY-TOKEN\n  description: Security token returned after creating a session.\n  sources:\n  - openapi/capital-com-public-api-capital-com-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capital-com-public-api/refs/heads/main/authentication/capital-com-public-api-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- CFD
- Commodities
- Cryptocurrency
- Financial
- Forex
- Indices
- Market Data
- Shares
- Streaming
- Trading
- WebSocket
---
