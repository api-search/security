---
api_key_in:
- query
api_specs:
- filename: finage-openapi.yml
  format: yaml
  label: Finage Market Data API
  slug: finage-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finage/refs/heads/main/openapi/finage-openapi.yml
- filename: finage-websocket-asyncapi.yml
  format: yaml
  label: Finage WebSocket Market Data Stream
  slug: finage-websocket-market-data-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/finage/refs/heads/main/asyncapi/finage-websocket-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Finage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Finage
provider_slug: finage
scheme_count: 1
schemes:
- description: Finage API key, passed as the apikey query parameter on every request. Get one at https://moon.finage.co.uk/register.
  in: query
  name: apiKey
  parameter: apikey
  sources:
  - openapi/finage-openapi.yml
  type: apiKey
slug: finage-authentication
source_filename: finage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: derived\nsource: openapi/finage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Finage API key, passed as the apikey query parameter on every request. Get one\n    at https://moon.finage.co.uk/register.\n  sources:\n  - openapi/finage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finage/refs/heads/main/authentication/finage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Market Data
- Stocks
- Forex
- Cryptocurrency
- ETFs
- Indices
- Fundamentals
- Real-Time Data
- Public APIs
---
