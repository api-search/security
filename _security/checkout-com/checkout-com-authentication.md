---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Checkout Com Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Checkout.com secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Checkout.com
provider_slug: checkout-com
scheme_count: 2
schemes:
- description: Secret API key as Bearer token (format `Bearer sk_...`).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/checkout-com-openapi.yml
  type: http
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://access.checkout.com/connect/token
  name: OAuth2
  sources:
  - openapi/checkout-com-openapi.yml
  type: oauth2
slug: checkout-com-authentication
source_filename: checkout-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkout-com-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Secret API key as Bearer token (format `Bearer sk_...`).\n  sources:\n  - openapi/checkout-com-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://access.checkout.com/connect/token\n    scopes: 2\n  description: OAuth 2.0 client credentials flow\n  sources:\n  - openapi/checkout-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/authentication/checkout-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fintech
- Payments
- Cards
- Acquiring
- Cross-Border
---
