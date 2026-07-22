---
api_key_in: []
api_specs:
- filename: teya-online-payments-openapi.yaml
  format: yaml
  label: Teya Online Payments API
  slug: teya-online-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-online-payments-openapi.yaml
- filename: teya-payments-openapi.yaml
  format: yaml
  label: Teya Payments Gateway API
  slug: teya-payments-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-payments-openapi.yaml
- filename: teya-poslink-openapi.json
  format: json
  label: Teya POSLink API
  slug: teya-poslink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-poslink-openapi.json
- filename: teya-fx-openapi.yaml
  format: yaml
  label: Teya FX (DCC) API
  slug: teya-fx-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-fx-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Teya Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Teya secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Teya
provider_slug: teya
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://id.teya.xyz/oauth/v2/oauth-authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token
  name: checkout_oauth_dev
  sources:
  - openapi/teya-online-payments-openapi.yaml
  - openapi/teya-payments-openapi.yaml
  type: oauth2
- flows:
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: Teya_Digital_Receipts_Service_oauth_prd
  sources:
  - openapi/teya-online-payments-openapi.yaml
  - openapi/teya-poslink-openapi.json
  type: oauth2
slug: teya-authentication
source_filename: teya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/teya-online-payments-openapi.yaml, openapi/teya-payments-openapi.yaml, openapi/teya-poslink-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: checkout_oauth_dev\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.xyz/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token\n    scopes: 0\n  sources:\n  - openapi/teya-online-payments-openapi.yaml\n  - openapi/teya-payments-openapi.yaml\n- name: Teya_Digital_Receipts_Service_oauth_prd\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n    scopes: 0\n  sources:\n  - openapi/teya-online-payments-openapi.yaml\n\
  \  - openapi/teya-poslink-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/authentication/teya-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Payments
- Payment Processing
- Card Acquiring
- Online Payments
- Point of Sale
- E-commerce
- Fintech
- Merchant Services
- Europe
---
