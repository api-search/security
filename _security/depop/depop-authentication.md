---
api_key_in:
- header
api_specs:
- filename: depop-selling-openapi-original.yml
  format: yaml
  label: Depop Selling API
  slug: depop-selling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depop/refs/heads/main/openapi/depop-selling-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Depop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: depop secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: depop
provider_slug: depop
scheme_count: 2
schemes:
- bearerFormat: API key
  description: 'Authorization: Bearer <token>. Token is either a static per-shop API key (prefix pak_) or a short-lived OAuth 2.0 access token.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/depop-selling-openapi-original.yml
  type: http
- description: OAuth 2.0 Authorization Code flow with mandatory PKCE (S256), per RFC 6749 and RFC 7636. Sellers grant granular scopes; access + refresh tokens are issued at the token endpoint.
  flows:
  - flow: authorizationCode
    pkce: S256
    scopes:
    - products_read
    - products_write
    - orders_read
    - orders_write
    - offers_read
    - offers_write
    - shop_read
    tokenUrl: https://partnerapi.depop.com/api/v1/oauth2/access-token/
  name: OAuth2
  source: https://partnerapi.depop.com/api-docs/concepts/authentication/
  type: oauth2
slug: depop-authentication
source_filename: depop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/depop-selling-openapi-original.yml\ndocs: https://partnerapi.depop.com/api-docs/concepts/authentication/\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    The OpenAPI declares a single http bearer scheme (BearerAuth). The docs\n    document two mechanisms: static per-shop API keys (bearer tokens prefixed\n    pak_) and OAuth 2.0 Authorization Code flow with PKCE (S256) for acting on\n    behalf of a Depop seller. API-key tokens carry all scopes; OAuth tokens are\n    limited to the scopes granted at authorization. Access is not self-service:\n    partners must be onboarded by Depop (developers@depop.com).\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: >-\n    Authorization: Bearer <token>. Token is either a static per-shop API key\n    (prefix pak_) or a short-lived OAuth 2.0 access token.\n\
  \  sources:\n  - openapi/depop-selling-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 Authorization Code flow with mandatory PKCE (S256), per RFC 6749\n    and RFC 7636. Sellers grant granular scopes; access + refresh tokens are\n    issued at the token endpoint.\n  flows:\n  - flow: authorizationCode\n    tokenUrl: https://partnerapi.depop.com/api/v1/oauth2/access-token/\n    pkce: S256\n    scopes:\n    - products_read\n    - products_write\n    - orders_read\n    - orders_write\n    - offers_read\n    - offers_write\n    - shop_read\n  source: https://partnerapi.depop.com/api-docs/concepts/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depop/refs/heads/main/authentication/depop-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Fashion
- Marketplace
- E-commerce
- Resale
- Retail
- Inventory Management
- Orders
- Sustainability
---
