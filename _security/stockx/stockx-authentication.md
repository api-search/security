---
api_key_in:
- header
api_specs:
- filename: stockx-public-openapi-original.json
  format: json
  label: StockX Public API
  slug: stockx-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/openapi/stockx-public-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Stockx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: StockX secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: StockX
provider_slug: stockx
scheme_count: 3
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/stockx-public-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  name: jwt
  scheme: bearer
  sources:
  - openapi/stockx-public-openapi-original.json
  type: http
- audience: gateway.stockx.com
  authorizationUrl: https://accounts.stockx.com/authorize
  flow: authorizationCode
  jwks_uri: https://accounts.stockx.com/.well-known/jwks.json
  name: oauth2
  scopes:
  - openid
  - offline_access
  source: https://accounts.stockx.com/.well-known/openid-configuration
  tokenUrl: https://accounts.stockx.com/oauth/token
  type: oauth2
slug: stockx-authentication
source_filename: stockx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/stockx-public-openapi-original.json\ndocs: https://developer.stockx.com/portal/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nnotes: >-\n  StockX Public API requires BOTH an x-api-key header AND an OAuth 2.0 bearer\n  access token on every request. Access tokens are issued by StockX's Auth0\n  tenant (accounts.stockx.com) via the Authorization Code flow; the audience\n  must be set to gateway.stockx.com. The API key is generated in the developer\n  portal once developer-program access is approved.\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/stockx-public-openapi-original.json\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/stockx-public-openapi-original.json\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl:\
  \ https://accounts.stockx.com/authorize\n  tokenUrl: https://accounts.stockx.com/oauth/token\n  jwks_uri: https://accounts.stockx.com/.well-known/jwks.json\n  audience: gateway.stockx.com\n  scopes:\n  - openid\n  - offline_access\n  source: https://accounts.stockx.com/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/authentication/stockx-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Marketplace
- E-Commerce
- Sneakers
- Streetwear
- Resale
- Collectibles
- Catalog
- Selling
- Orders
---
