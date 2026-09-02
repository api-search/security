---
api_key_in: []
api_specs:
- filename: clover-charges-api-openapi.yml
  format: yaml
  label: Clover CHARGES API
  slug: clover-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-charges-api-openapi.yml
- filename: clover-checkout-api-openapi.yml
  format: yaml
  label: Clover CHECKOUT API
  slug: clover-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-checkout-api-openapi.yml
- filename: clover-customers-api-openapi.yml
  format: yaml
  label: Clover CUSTOMERS API
  slug: clover-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-customers-api-openapi.yml
- filename: clover-employees-api-openapi.yml
  format: yaml
  label: Clover EMPLOYEES API
  slug: clover-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-employees-api-openapi.yml
- filename: clover-inventory-api-openapi.yml
  format: yaml
  label: Clover INVENTORY API
  slug: clover-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-inventory-api-openapi.yml
- filename: clover-orders-api-openapi.yml
  format: yaml
  label: Clover ORDERS API
  slug: clover-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-orders-api-openapi.yml
- filename: clover-payments-api-openapi.yml
  format: yaml
  label: Clover PAYMENTS API
  slug: clover-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-payments-api-openapi.yml
- filename: clover-refunds-api-openapi.yml
  format: yaml
  label: Clover REFUNDS API
  slug: clover-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-refunds-api-openapi.yml
- filename: clover-tokens-api-openapi.yml
  format: yaml
  label: Clover TOKENS API
  slug: clover-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-tokens-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Clover Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Clover secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Clover
provider_slug: clover
scheme_count: 2
schemes:
- description: OAuth 2.0 token or Ecommerce (PAKMS) API key.
  flows:
  - authorizationUrl: https://www.clover.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.clover.com/oauth/token
  name: OAuth2
  sources:
  - openapi/clover-ecommerce-api-openapi.yml
  type: oauth2
- description: OAuth 2.0 access token or merchant API token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clover-platform-rest-api-openapi.yml
  type: http
slug: clover-authentication
source_filename: clover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clover-ecommerce-api-openapi.yml, openapi/clover-platform-rest-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.clover.com/oauth/authorize\n    tokenUrl: https://api.clover.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 token or Ecommerce (PAKMS) API key.\n  sources:\n  - openapi/clover-ecommerce-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token or merchant API token.\n  sources:\n  - openapi/clover-platform-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/authentication/clover-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Restaurant
- Point-of-Sale
- Payments
- Retail
- SMB
- Hardware
---
