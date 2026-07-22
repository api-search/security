---
api_key_in: []
api_specs:
- filename: logiless-openapi.yml
  format: yaml
  label: LOGILESS API
  slug: logiless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Logiless Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Logiless secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Logiless
provider_slug: logiless
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  sources:
  - openapi/logiless-openapi.yml
  type: oauth2
slug: logiless-authentication
source_filename: logiless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/logiless-openapi.yml\ndocs: https://app2.logiless.com/developer/documents/authentication\nnotes: >-\n  OAuth 2.0 authorization-code flow (RFC 6749 / RFC 6750). Applications must be\n  registered and pass a 3–5 business-day review in the LOGILESS Developers console\n  before receiving a client_id / client_secret. Access tokens are sent as\n  `Authorization: Bearer {token}`. Both access and refresh tokens expire after 30\n  days (expires_in = 2592000). Authorization codes expire after 10 minutes and are\n  single-use. Tokens are issued per LOGILESS user; API data is limited to the\n  merchant that user belongs to. An optional access-range restriction can pin a\n  token to a specific merchant_id / store_id at authorization time. There is no\n  OAuth scope surface (the `scope` field is returned empty); access is governed by\n  merchant/store membership instead.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n\
  \  token_ttl_seconds: 2592000\n  refresh_supported: true\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\n  sources:\n  - openapi/logiless-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/authentication/logiless-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Logistics
- E-commerce
- Order Management
- Warehouse Management
- Inventory
- Fulfillment
- Shipping
- OMS
- WMS
- Japan
---
