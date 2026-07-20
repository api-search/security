---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kartrocket Authentication
name_suffix: Authentication
oauth_flows: []
overview: KartRocket secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KartRocket
provider_slug: kartrocket
scheme_count: 1
schemes:
- bearer_format: JWT
  header: Authorization
  in: header
  name: bearerAuth
  obtain:
    body:
      email: <seller-email>
      password: <seller-password>
    method: POST
    returns: token
    url: https://apiv2.shiprocket.in/v1/external/auth/login
  scheme: bearer
  sources:
  - apidocs.shiprocket.in
  - github.com/bfrs/shiprocket-mcp
  token_lifetime: ~10 days (re-login on expiry)
  type: http
slug: kartrocket-authentication
source_filename: kartrocket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apidocs.shiprocket.in/ + https://github.com/bfrs/shiprocket-mcp\ndocs: https://apidocs.shiprocket.in/\nsummary:\n  types: [http]\n  scheme: bearer\n  token_source: login-endpoint\n  oauth2_flows: []\nnotes: >-\n  Shiprocket's public API uses token (JWT) bearer auth. The seller POSTs email +\n  password to the login endpoint and receives a bearer token used on every\n  subsequent request as `Authorization: Bearer <token>`. Confirmed by the official\n  MCP server, which takes SELLER_EMAIL + SELLER_PASSWORD and logs in on the seller's\n  behalf. No OAuth2 authorization-code flow and no static API keys are documented;\n  the login token is the credential.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n    obtain:\n      method: POST\n      url: https://apiv2.shiprocket.in/v1/external/auth/login\n      body: { email: <seller-email>,\
  \ password: <seller-password> }\n      returns: token\n    token_lifetime: ~10 days (re-login on expiry)\n    sources: [apidocs.shiprocket.in, github.com/bfrs/shiprocket-mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kartrocket/refs/heads/main/authentication/kartrocket-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Shipping
- Logistics
- eCommerce
- Fulfillment
- Last-Mile Delivery
- India
- Order Management
---
