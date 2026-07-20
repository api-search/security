---
api_key_in:
- header
api_specs:
- filename: carry1st-pay1st-gateway-openapi.yml
  format: yaml
  label: Pay1st Gateway API
  slug: pay1st-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carry1st/refs/heads/main/openapi/carry1st-pay1st-gateway-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Carry1St Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carry1st secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Carry1st
provider_slug: carry1st
scheme_count: 2
schemes:
- description: Base64(API_KEY:API_SECRET) used only on the auth/token and auth/refresh endpoints.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/carry1st-pay1st-gateway-openapi.yml
  type: http
- description: Bearer <AccessToken> issued by generateAccessToken; required on all Gateway API requests.
  in: header
  name: accessToken
  parameter: AccessToken
  sources:
  - openapi/carry1st-pay1st-gateway-openapi.yml
  type: apiKey
slug: carry1st-authentication
source_filename: carry1st-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/carry1st-pay1st-gateway-openapi.yml\ndocs: https://pay1st-docs.carry1st.com/reference/configuring-api-credentials\nnotes: >-\n  Two-stage model. Stage 1: an API Key + API Secret (HTTP Basic, Base64(API_KEY:API_SECRET))\n  authenticates the /api/pay1st/auth/token call to mint a short-lived Access Token plus a\n  Refresh Token. Stage 2: every other Gateway request carries the Access Token in the\n  AccessToken header as \"Bearer <AccessToken>\", and every mutating request is additionally\n  signed with a hex HMAC-SHA256 X-SIGNATURE (over X-TIMESTAMP + request JSON, keyed by the\n  Signing Key) to prove the payload was not tampered with. Credentials are generated in the\n  Pay1st Console.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Base64(API_KEY:API_SECRET) used only on the auth/token and auth/refresh endpoints.\n  sources:\n\
  \  - openapi/carry1st-pay1st-gateway-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: AccessToken\n  description: Bearer <AccessToken> issued by generateAccessToken; required on all Gateway API\n    requests.\n  sources:\n  - openapi/carry1st-pay1st-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carry1st/refs/heads/main/authentication/carry1st-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Payments
- Payment Gateway
- Fintech
- Gaming
- Mobile Games
- Africa
- Digital Commerce
- Merchant of Record
- Games Publishing
---
