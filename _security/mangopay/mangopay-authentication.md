---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Mangopay REST API
  slug: mangopay-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mangopay/refs/heads/main/openapi/openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mangopay Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Mangopay secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Mangopay
provider_slug: mangopay
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.mangopay.com/v2.01/{clientId}/oauth/token
  name: OAuth2
  sources:
  - openapi/openapi.json
  type: oauth2
slug: mangopay-authentication
source_filename: mangopay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.mangopay.com/v2.01/{clientId}/oauth/token\n    scopes: 0\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mangopay/refs/heads/main/authentication/mangopay-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Payments
- Marketplace Payments
- Digital Wallets
- KYC
- KYB
- Fund Transfers
- Currency Conversion
- Payment Cards
- Fintech
- European
---
