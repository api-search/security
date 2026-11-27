---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-shopping-accounts-api-openapi.yml
  format: yaml
  label: Google Content API for Shopping Accounts API
  slug: google-shopping-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-shopping/openapi/google-shopping-accounts-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Content API for Shopping Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Content API for Shopping secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Content API for Shopping
provider_slug: google-shopping
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-shopping-accounts-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-shopping-accounts-api-openapi.yml
  type: oauth2
slug: google-shopping-authentication
source_filename: google-shopping-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-shopping-accounts-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-shopping-accounts-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/google-shopping-accounts-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-shopping/authentication/google-shopping-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- E-Commerce
- Google Shopping
- Merchant Center
- Product Listings
- Retail
- Shopping
---
