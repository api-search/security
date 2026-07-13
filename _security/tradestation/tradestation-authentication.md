---
api_key_in: []
api_specs:
- filename: tradestation-api-openapi.yml
  format: yaml
  label: TradeStation API
  slug: tradestation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/openapi/tradestation-api-openapi.yml
- filename: tradestation-streaming-asyncapi.yml
  format: yaml
  label: TradeStation Streaming API
  slug: tradestation-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/asyncapi/tradestation-streaming-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tradestation Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TradeStation secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TradeStation
provider_slug: tradestation
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization code flow for accessing TradeStation API resources. Requires user authorization and supports token refresh.
  flows:
  - authorizationUrl: https://signin.tradestation.com/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://signin.tradestation.com/oauth/token
  name: oauth2AuthCode
  sources:
  - openapi/tradestation-api-openapi.yml
  type: oauth2
slug: tradestation-authentication
source_filename: tradestation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tradestation-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2AuthCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://signin.tradestation.com/authorize\n    tokenUrl: https://signin.tradestation.com/oauth/token\n    scopes: 3\n  description: OAuth 2.0 authorization code flow for accessing TradeStation API resources. Requires\n    user authorization and supports token refresh.\n  sources:\n  - openapi/tradestation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/authentication/tradestation-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Brokerage
- Cryptocurrency
- Finance
- Futures
- Market Data
- Options
- Stocks
- Trading
---
