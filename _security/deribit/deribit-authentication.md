---
api_key_in: []
api_specs:
- filename: deribit_openapi.json
  format: json
  label: Deribit REST API
  slug: deribit-rest-api
  spec_type: OpenAPI
  url: https://docs.deribit.com/specifications/deribit_openapi.json
- filename: asyncapi.yaml
  format: yaml
  label: Deribit WebSocket API
  slug: deribit-websocket-api
  spec_type: AsyncAPI
  url: https://docs.deribit.com/
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deribit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deribit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deribit
provider_slug: deribit
scheme_count: 1
schemes:
- description: API key passed as a Bearer token. The authenticated session determines the portfolio that operations are applied to.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/deribit-starbase-openapi.json
  type: http
slug: deribit-authentication
source_filename: deribit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deribit-starbase-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token. The authenticated session determines the portfolio\n    that operations are applied to.\n  sources:\n  - openapi/deribit-starbase-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/authentication/deribit-authentication.yml
summary_line: http · 1 scheme
tags:
- Derivatives
- Cryptocurrency
- Bitcoin
- Ethereum
- Options
- Futures
- Perpetuals
- Trading
- Market Data
- Block Trading
- WebSocket
- Financial
---
