---
api_key_in:
- header
api_specs:
- filename: loop-returns-returns-openapi.yml
  format: yaml
  label: Loop Returns API
  slug: loop-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop-returns/refs/heads/main/openapi/loop-returns-returns-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Loop Returns Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Loop Returns secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Loop Returns
provider_slug: loop-returns
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: X-Authorization
  sources:
  - openapi/loop-returns-carts-openapi.yml
  - openapi/loop-returns-destinations-openapi.yml
  - openapi/loop-returns-fraud-reports-openapi.yml
  - openapi/loop-returns-labels-openapi.yml
  - openapi/loop-returns-returns-openapi.yml
  - openapi/loop-returns-webhooks-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://oauth.loopreturns.com/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://oauth.loopreturns.com/oauth/token
  name: oauth2
  sources:
  - openapi/loop-returns-labels-openapi.yml
  - openapi/loop-returns-webhooks-openapi.yml
  type: oauth2
slug: loop-returns-authentication
source_filename: loop-returns-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loop-returns-carts-openapi.yml, openapi/loop-returns-destinations-openapi.yml,\n  openapi/loop-returns-fraud-reports-openapi.yml, openapi/loop-returns-labels-openapi.yml, openapi/loop-returns-returns-openapi.yml,\n  openapi/loop-returns-webhooks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Authorization\n  sources:\n  - openapi/loop-returns-carts-openapi.yml\n  - openapi/loop-returns-destinations-openapi.yml\n  - openapi/loop-returns-fraud-reports-openapi.yml\n  - openapi/loop-returns-labels-openapi.yml\n  - openapi/loop-returns-returns-openapi.yml\n  - openapi/loop-returns-webhooks-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.loopreturns.com/authorize\n    tokenUrl: https://oauth.loopreturns.com/oauth/token\n\
  \    scopes: 5\n  sources:\n  - openapi/loop-returns-labels-openapi.yml\n  - openapi/loop-returns-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loop-returns/refs/heads/main/authentication/loop-returns-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Returns
- E-Commerce
- Exchanges
- Refunds
- Shipping
- Post-Purchase
- Shopify
- Fraud Prevention
- Retail
---
