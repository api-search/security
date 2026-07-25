---
api_key_in: []
api_specs:
- filename: salla-webhooks-asyncapi.yml
  format: yaml
  label: Salla Webhooks
  slug: salla-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-webhooks-asyncapi.yml
- filename: salla-branches-api-openapi.yml
  format: yaml
  label: Salla Branches API
  slug: salla-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-branches-api-openapi.yml
- filename: salla-brands-api-openapi.yml
  format: yaml
  label: Salla Brands API
  slug: salla-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-brands-api-openapi.yml
- filename: salla-carts-api-openapi.yml
  format: yaml
  label: Salla Carts API
  slug: salla-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-carts-api-openapi.yml
- filename: salla-categories-api-openapi.yml
  format: yaml
  label: Salla Categories API
  slug: salla-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-categories-api-openapi.yml
- filename: salla-coupons-api-openapi.yml
  format: yaml
  label: Salla Coupons API
  slug: salla-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-coupons-api-openapi.yml
- filename: salla-customers-api-openapi.yml
  format: yaml
  label: Salla Customers API
  slug: salla-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-customers-api-openapi.yml
- filename: salla-financial-api-openapi.yml
  format: yaml
  label: Salla Financial API
  slug: salla-financial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-financial-api-openapi.yml
- filename: salla-localization-api-openapi.yml
  format: yaml
  label: Salla Localization API
  slug: salla-localization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-localization-api-openapi.yml
- filename: salla-oauth-api-openapi.yml
  format: yaml
  label: Salla OAuth API
  slug: salla-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-oauth-api-openapi.yml
- filename: salla-orders-api-openapi.yml
  format: yaml
  label: Salla Orders API
  slug: salla-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-orders-api-openapi.yml
- filename: salla-products-api-openapi.yml
  format: yaml
  label: Salla Products API
  slug: salla-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-products-api-openapi.yml
- filename: salla-shipments-api-openapi.yml
  format: yaml
  label: Salla Shipments API
  slug: salla-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-shipments-api-openapi.yml
- filename: salla-shipping-api-openapi.yml
  format: yaml
  label: Salla Shipping API
  slug: salla-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-shipping-api-openapi.yml
- filename: salla-store-api-openapi.yml
  format: yaml
  label: Salla Store API
  slug: salla-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-store-api-openapi.yml
- filename: salla-webhooks-api-openapi.yml
  format: yaml
  label: Salla Webhooks API
  slug: salla-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-webhooks-api-openapi.yml
- filename: salla-zones-api-openapi.yml
  format: yaml
  label: Salla Zones API
  slug: salla-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-zones-api-openapi.yml
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
