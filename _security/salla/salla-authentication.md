---
api_key_in: []
api_specs:
- filename: salla-merchant-api-openapi.yml
  format: yaml
  label: Salla Merchant API
  slug: salla-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-merchant-api-openapi.yml
- filename: salla-apps-api-openapi.yml
  format: yaml
  label: Salla Apps API
  slug: salla-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-apps-api-openapi.yml
- filename: salla-shipping-fulfillment-api-openapi.yml
  format: yaml
  label: Salla Shipping and Fulfillment API
  slug: salla-shipping-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-shipping-fulfillment-api-openapi.yml
- filename: salla-webhooks-asyncapi.yml
  format: yaml
  label: Salla Webhooks
  slug: salla-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-webhooks-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salla Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salla secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salla
provider_slug: salla
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/salla-apps-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://accounts.salla.sa/oauth2/auth
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://accounts.salla.sa/oauth2/token
  name: OAuth2
  sources:
  - openapi/salla-merchant-api-openapi.yml
  - openapi/salla-shipping-fulfillment-api-openapi.yml
  type: oauth2
slug: salla-authentication
source_filename: salla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salla-apps-api-openapi.yml, openapi/salla-merchant-api-openapi.yml, openapi/salla-shipping-fulfillment-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/salla-apps-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.salla.sa/oauth2/auth\n    tokenUrl: https://accounts.salla.sa/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n  - openapi/salla-shipping-fulfillment-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/authentication/salla-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Arabic
- E-Commerce
- GCC
- Headless Commerce
- Merchant
- MENA
- Online Stores
- Retail
- Saudi Arabia
- SMB
- Storefront
---
