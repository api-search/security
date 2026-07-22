---
api_key_in: []
api_specs:
- filename: ual-bis-cobros-online-v2-openapi.yml
  format: yaml
  label: Ualá Bis API Cobros Online v2
  slug: ualá-bis-api-cobros-online-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/openapi/ual-bis-cobros-online-v2-openapi.yml
- filename: ual-bis-auth-v2-openapi.yml
  format: yaml
  label: Ualá Bis Authentication API v2
  slug: ualá-bis-authentication-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/openapi/ual-bis-auth-v2-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ual Authentication
name_suffix: Authentication
oauth_flows:
- client_credentials (custom JSON body, non-RFC 6749 encoding)
overview: Ualá secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the client_credentials (custom JSON body, non-RFC 6749 encoding) flow(s).
provider_name: Ualá
provider_slug: ual
scheme_count: 1
schemes:
- description: 'All Ualá Bis Cobros Online v2 endpoints require Authorization: Bearer <token>. The token is created via POST /auth/token on https://auth.developers.ar.ua.la/v2/api (test: https://auth.stage.developers.ar.ua.la/v2/api) with a JSON body of username, client_id, client_secret_id and grant_type=client_credentials — an OAuth2-style client-credentials exchange carried in custom JSON rather than RFC 6749 form encoding. Credentials for both test and production are issued in the Ualá Bis welcome email and shown in the mobile/web apps; they are private and Ualá staff never request them.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ual-bis-cobros-online-v2-openapi.yml
  - openapi/ual-bis-auth-v2-openapi.yml
  token_endpoint:
    production: https://auth.developers.ar.ua.la/v2/api/auth/token
    test: https://auth.stage.developers.ar.ua.la/v2/api/auth/token
  type: http
slug: ual-authentication
source_filename: ual-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.ualabis.com.ar/v2/authentication/create\ndocs: https://developers.ualabis.com.ar/v2/authentication/create\nsummary:\n  types:\n  - http\n  oauth2_flows:\n  - client_credentials (custom JSON body, non-RFC 6749 encoding)\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    All Ualá Bis Cobros Online v2 endpoints require Authorization: Bearer <token>. The token\n    is created via POST /auth/token on https://auth.developers.ar.ua.la/v2/api (test:\n    https://auth.stage.developers.ar.ua.la/v2/api) with a JSON body of username, client_id,\n    client_secret_id and grant_type=client_credentials — an OAuth2-style client-credentials\n    exchange carried in custom JSON rather than RFC 6749 form encoding. Credentials for both\n    test and production are issued in the Ualá Bis welcome email and shown in the mobile/web\n    apps; they are private and Ualá staff never request them.\n\
  \  token_endpoint:\n    production: https://auth.developers.ar.ua.la/v2/api/auth/token\n    test: https://auth.stage.developers.ar.ua.la/v2/api/auth/token\n  sources:\n  - openapi/ual-bis-cobros-online-v2-openapi.yml\n  - openapi/ual-bis-auth-v2-openapi.yml\nnotes: >-\n  No API-key or OpenID Connect surface; no OAuth scopes are documented (scopes/ intentionally\n  omitted).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/authentication/ual-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Banking
- Neobank
- Checkout
- Ecommerce
- Argentina
- Mexico
---
