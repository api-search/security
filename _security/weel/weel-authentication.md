---
api_key_in: []
api_specs:
- filename: weel-openapi.yml
  format: yaml
  label: Weel Open API
  slug: weel-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Weel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weel
provider_slug: weel
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/weel-openapi.yml
  type: http
slug: weel-authentication
source_filename: weel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/weel-openapi.yml\ndocs: https://developer.letsweel.com/getting-started/authentication\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/weel-openapi.yml\ndetails:\n  token_type: API key (bearer)\n  header: 'Authorization: Bearer <token>'\n  creation: >-\n    Created in the Weel web app under Settings > API > Create New API Key\n    (https://app.letsweel.com/app/settings#api).\n  expiry: >-\n    Bearer tokens do not expire. They remain valid until revoked or replaced\n    (delete the token under Settings > API).\n  rotation: Manual — revoke and recreate in-app; no programmatic rotation endpoint.\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  gating: API access is an Enterprise-plan capability.\nnotes: >-\n  Single security scheme across all operations: HTTP\
  \ bearer token. No OAuth2,\n  OpenID Connect, or mutual TLS is documented, and no OAuth/OIDC discovery\n  metadata is served — so there is no scope surface (hence no scopes/ artifact).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/authentication/weel-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Australia
- Spend Management
- Expense Management
- Corporate Cards
- Accounts Payable
- Card Issuing
- Reimbursements
- Budgets
- Fintech
---
