---
api_key_in: []
api_specs:
- filename: bread-pay-platform-openapi.yml
  format: yaml
  label: Bread Pay Platform API
  slug: bread-pay-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/openapi/bread-pay-platform-openapi.yml
- filename: bread-classic-merchant-openapi.yml
  format: yaml
  label: Bread Classic Merchant API
  slug: bread-classic-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/openapi/bread-classic-merchant-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Alliance Data Systems Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Alliance Data Systems (Bread Financial Holdings) secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Alliance Data Systems (Bread Financial Holdings)
provider_slug: alliance-data-systems
scheme_count: 2
schemes:
- description: Bread Merchant Portal access token (legacy scheme).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bread-classic-merchant-openapi.yml
  type: http
- description: OAuth 2.0 Client Credentials flow using API + Secret keys issued from the Bread Merchant Portal.
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://auth.platform.breadpayments.com/auth/sso/token
  name: oauth2ClientCredentials
  sources:
  - openapi/bread-pay-platform-openapi.yml
  type: oauth2
slug: alliance-data-systems-authentication
source_filename: alliance-data-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bread-classic-merchant-openapi.yml, openapi/bread-pay-platform-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bread Merchant Portal access token (legacy scheme).\n  sources:\n  - openapi/bread-classic-merchant-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.platform.breadpayments.com/auth/sso/token\n    scopes: 3\n  description: OAuth 2.0 Client Credentials flow using API + Secret keys issued from the Bread\n    Merchant Portal.\n  sources:\n  - openapi/bread-pay-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/authentication/alliance-data-systems-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Financial Services
- Fintech
- Buy Now Pay Later
- BNPL
- Bread Pay
- Private Label Credit
- Co Brand Credit Cards
- Loyalty Programs
- Marketing
- Data Driven Marketing
- Payments
- Lending
- Savings
- Personal Loans
- Consumer Banking
- Retail Finance
- Fortune 500
- NYSE BFH
- Comenity Bank
- Rebrand
---
