---
api_key_in: []
api_specs:
- filename: thrivecart-api-openapi.yml
  format: yaml
  label: ThriveCart API
  slug: thrivecart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Thrivecart Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ThriveCart secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ThriveCart
provider_slug: thrivecart
scheme_count: 2
schemes:
- description: 'Account-scoped API key created under Settings > API & webhooks > API tokens, or an OAuth access token, sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/thrivecart-api-openapi.yml
  type: http
- description: OAuth 2.0 authorization code grant for applications acting on behalf of another ThriveCart account. ThriveCart does not publish a scope reference; access is granted account-wide on consent.
  flows:
  - authorizationUrl: https://thrivecart.com/authorization/new
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://thrivecart.com/authorization/token
  name: oauth2
  sources:
  - openapi/thrivecart-api-openapi.yml
  type: oauth2
slug: thrivecart-authentication
source_filename: thrivecart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/thrivecart-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Account-scoped API key created under Settings > API & webhooks > API tokens,\n    or an OAuth access token, sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/thrivecart-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://thrivecart.com/authorization/new\n    tokenUrl: https://thrivecart.com/authorization/token\n    scopes: 0\n  description: OAuth 2.0 authorization code grant for applications acting on behalf of another\n    ThriveCart account. ThriveCart does not publish a scope reference; access is granted account-wide\n    on consent.\n  sources:\n  - openapi/thrivecart-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/authentication/thrivecart-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Checkout
- Shopping Cart
- Payments
- E-Commerce
- Subscription
- Affiliate Marketing
- Learning Management
- Creator Economy
- Webhook
---
