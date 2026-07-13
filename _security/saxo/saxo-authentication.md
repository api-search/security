---
api_key_in: []
api_specs:
- filename: trade.yaml
  format: yaml
  label: Saxo Bank OpenAPI
  slug: saxo-bank-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/openapi/trade.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Saxo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Saxo Bank secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Saxo Bank
provider_slug: saxo
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: OpenApiJWTSecurityScheme
  scheme: bearer
  sources:
  - openapi/at.yaml
  - openapi/atr.yaml
  - openapi/ca.yaml
  - openapi/chart.yaml
  - openapi/cm.yaml
  - openapi/cr.yaml
  - openapi/cs.yaml
  - openapi/developer.yaml
  - openapi/ens.yaml
  - openapi/hist.yaml
  - openapi/mkt.yaml
  - openapi/partnerintegration.yaml
  - openapi/port.yaml
  - openapi/ref.yaml
  - openapi/root.yaml
  - openapi/trade.yaml
  - openapi/vas.yaml
  type: http
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  sources:
  - openapi/at.yaml
  - openapi/atr.yaml
  - openapi/ca.yaml
  - openapi/chart.yaml
  - openapi/cm.yaml
  - openapi/cr.yaml
  - openapi/cs.yaml
  - openapi/developer.yaml
  - openapi/ens.yaml
  - openapi/hist.yaml
  - openapi/mkt.yaml
  - openapi/partnerintegration.yaml
  - openapi/port.yaml
  - openapi/ref.yaml
  - openapi/root.yaml
  - openapi/trade.yaml
  - openapi/vas.yaml
  type: oauth2
slug: saxo-authentication
source_filename: saxo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/at.yaml, openapi/atr.yaml, openapi/ca.yaml, openapi/chart.yaml, openapi/cm.yaml,\n  openapi/cr.yaml, openapi/cs.yaml, openapi/developer.yaml, openapi/ens.yaml, openapi/hist.yaml,\n  openapi/mkt.yaml, openapi/partnerintegration.yaml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OpenApiJWTSecurityScheme\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/at.yaml\n  - openapi/atr.yaml\n  - openapi/ca.yaml\n  - openapi/chart.yaml\n  - openapi/cm.yaml\n  - openapi/cr.yaml\n  - openapi/cs.yaml\n  - openapi/developer.yaml\n  - openapi/ens.yaml\n  - openapi/hist.yaml\n  - openapi/mkt.yaml\n  - openapi/partnerintegration.yaml\n  - openapi/port.yaml\n  - openapi/ref.yaml\n  - openapi/root.yaml\n  - openapi/trade.yaml\n  - openapi/vas.yaml\n- name: OpenApiOAuthSecurityScheme\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n    scopes: 0\n  sources:\n  - openapi/at.yaml\n  - openapi/atr.yaml\n  - openapi/ca.yaml\n  - openapi/chart.yaml\n  - openapi/cm.yaml\n  - openapi/cr.yaml\n  - openapi/cs.yaml\n  - openapi/developer.yaml\n  - openapi/ens.yaml\n  - openapi/hist.yaml\n  - openapi/mkt.yaml\n  - openapi/partnerintegration.yaml\n  - openapi/port.yaml\n  - openapi/ref.yaml\n  - openapi/root.yaml\n  - openapi/trade.yaml\n  - openapi/vas.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/authentication/saxo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Investment Banking
- Trading
- Equities
- Forex
- Options
- Futures
- Market Data
- Portfolio Management
- Orders
- Financial
---
