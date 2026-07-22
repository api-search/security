---
api_key_in: []
auth_types:
- http
description: 'Thinknum uses token-based authentication over HTTPS to data.thinknum.com. Clients first exchange a client_id + client_secret (issued by a Thinknum account manager) for a short-lived bearer token via POST /api/authorize, then send that token on every request as `Authorization: token <TOKEN>` alongside a dated `X-API-Version` header. Tokens expire and must be re-obtained. Embeddable widgets use a separate HTTP Basic exchange (client_id:client_secret) against www.thinknum.com/authenticate that returns a 15-minute widget token.'
kind: authentication
layout: security
method: searched
name: Thinknum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thinknum secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thinknum
provider_slug: thinknum
scheme_count: 2
schemes:
- description: 'Bearer token issued by POST /api/authorize (body: client_id, client_secret, version). Response returns auth_token + auth_expires; token has a finite expiration and must be renewed.'
  format: token <TOKEN>
  header: Authorization
  in: header
  name: tokenAuth
  scheme: token
  source: https://docs.thinknum.com/docs/authenticating.md
  type: http
- description: HTTP Basic (client_id:client_secret) against https://www.thinknum.com/authenticate to mint a 15-minute token for the embeddable Company Metrics and Connections Map widgets. Requires a widget-activated client_id/client_secret.
  name: widgetBasicAuth
  scheme: basic
  source: https://docs.thinknum.com/docs/company-metrics-widget.md
  type: http
slug: thinknum-authentication
source_filename: thinknum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.thinknum.com/docs/authenticating.md\ndocs: https://docs.thinknum.com/docs/authenticating.md\ndescription: >-\n  Thinknum uses token-based authentication over HTTPS to data.thinknum.com.\n  Clients first exchange a client_id + client_secret (issued by a Thinknum\n  account manager) for a short-lived bearer token via POST /api/authorize, then\n  send that token on every request as `Authorization: token <TOKEN>` alongside a\n  dated `X-API-Version` header. Tokens expire and must be re-obtained. Embeddable\n  widgets use a separate HTTP Basic exchange (client_id:client_secret) against\n  www.thinknum.com/authenticate that returns a 15-minute widget token.\nsummary:\n  types:\n  - http\n  http_scheme: token\n  token_endpoint: https://data.thinknum.com/api/authorize\n  required_headers:\n  - name: Authorization\n    value: token <TOKEN>\n  - name: X-API-Version\n    value: '20151130'\nschemes:\n  - name: tokenAuth\n\
  \    type: http\n    scheme: token\n    in: header\n    header: Authorization\n    format: 'token <TOKEN>'\n    description: >-\n      Bearer token issued by POST /api/authorize (body: client_id, client_secret,\n      version). Response returns auth_token + auth_expires; token has a finite\n      expiration and must be renewed.\n    source: https://docs.thinknum.com/docs/authenticating.md\n  - name: widgetBasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic (client_id:client_secret) against\n      https://www.thinknum.com/authenticate to mint a 15-minute token for the\n      embeddable Company Metrics and Connections Map widgets. Requires a\n      widget-activated client_id/client_secret.\n    source: https://docs.thinknum.com/docs/company-metrics-widget.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thinknum/refs/heads/main/authentication/thinknum-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Alternative Data
- Financial Data
- Investment Research
- Market Intelligence
- Web Data
- Datasets
---
