---
api_key_in: []
api_specs:
- filename: vori-openapi.yml
  format: yaml
  label: Vori API
  slug: vori-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vori/refs/heads/main/openapi/vori-openapi.yml
auth_types:
- http
description: 'Every Vori REST API request carries a bearer JWT in the Authorization header. There is no Vori-issued API key or OAuth flow: integrations exchange a Vori user''s email/password at Google Identity Toolkit (Firebase identitytoolkit/v3/relyingparty/verifyPassword) for an idToken, then refresh hourly by exchanging the returned refreshToken at securetoken.googleapis.com/v1/token (refresh tokens may rotate on each exchange). Vori recommends creating a banner-level Read-only role user for read-only integrations to limit blast radius.'
kind: authentication
layout: security
method: searched
name: Vori Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vori secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vori
provider_slug: vori
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/vori-openapi.yml
  type: http
slug: vori-authentication
source_filename: vori-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/vori-openapi.yml\ndocs: https://help.vori.com/api/introduction\nsummary:\n  types:\n  - http\ndescription: >-\n  Every Vori REST API request carries a bearer JWT in the Authorization header.\n  There is no Vori-issued API key or OAuth flow: integrations exchange a Vori\n  user's email/password at Google Identity Toolkit (Firebase\n  identitytoolkit/v3/relyingparty/verifyPassword) for an idToken, then refresh\n  hourly by exchanging the returned refreshToken at\n  securetoken.googleapis.com/v1/token (refresh tokens may rotate on each\n  exchange). Vori recommends creating a banner-level Read-only role user for\n  read-only integrations to limit blast radius.\ntoken_flow:\n  obtain: POST https://www.googleapis.com/identitytoolkit/v3/relyingparty/verifyPassword (email, password, returnSecureToken)\n  refresh: POST https://securetoken.googleapis.com/v1/token (grant_type=refresh_token)\n  lifetime: idToken expires after\
  \ one hour\n  header: 'Authorization: Bearer <idToken>'\nleast_privilege:\n  recommendation: banner-level Read-only role account for read-only integrations\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/vori-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vori/refs/heads/main/authentication/vori-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Applications
- Grocery
- Point of Sale
- Retail
- Inventory
- Payments
- Commerce
---
