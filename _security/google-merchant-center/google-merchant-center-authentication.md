---
api_key_in: []
api_specs:
- filename: google-merchant-center-accounts-api-openapi.yml
  format: yaml
  label: Google Merchant Center Accounts API
  slug: google-merchant-center-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-accounts-api-openapi.yml
- filename: google-merchant-center-inventories-api-openapi.yml
  format: yaml
  label: Google Merchant Center Inventories API
  slug: google-merchant-center-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-inventories-api-openapi.yml
- filename: google-merchant-center-products-api-openapi.yml
  format: yaml
  label: Google Merchant Center Products API
  slug: google-merchant-center-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-products-api-openapi.yml
- filename: google-merchant-center-promotions-api-openapi.yml
  format: yaml
  label: Google Merchant Center Promotions API
  slug: google-merchant-center-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-promotions-api-openapi.yml
- filename: google-merchant-center-reports-api-openapi.yml
  format: yaml
  label: Google Merchant Center Reports API
  slug: google-merchant-center-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-reports-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Merchant Center Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Merchant Center secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Merchant Center
provider_slug: google-merchant-center
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-merchant-center-authentication
source_filename: google-merchant-center-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/authentication/google-merchant-center-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- E-Commerce
- Google Shopping
- Inventory
- Merchant Center
- Product
- Promotions
- Shopping
---
