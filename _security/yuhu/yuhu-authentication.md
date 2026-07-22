---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Yuhu Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Yuhu secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Yuhu
provider_slug: yuhu
scheme_count: 1
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  revocation_url: https://api.yuhu.io/partners/revoke
  sources:
  - https://developer.yuhu.io/
  token_type: Bearer
  token_url: https://api.yuhu.io/partners/token
  type: oauth2
slug: yuhu-authentication
source_filename: yuhu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.yuhu.io/\ndocs: https://developer.yuhu.io/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\nnotes: >-\n  Yuhu Partners API uses OAuth 2.0 client-credentials. Partners exchange a client_id and\n  client_secret for a bearer access token, then send it as an Authorization: Bearer header\n  on all v1 requests. Tokens can be revoked. No user-delegated flows or API keys are\n  documented; there is no documented OAuth scope surface (client-credentials only).\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.yuhu.io/partners/token\n  revocation_url: https://api.yuhu.io/partners/revoke\n  grant_type: client_credentials\n  token_type: Bearer\n  sources: [https://developer.yuhu.io/]\ntoken_endpoint:\n  method: POST\n  url: https://api.yuhu.io/partners/token\n  params: [grant_type=client_credentials, client_id, client_secret]\n\
  \  headers:\n    Content-Type: application/json\n    Accept: application/json\n  response_fields: [access_token, token_type, created_at]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuhu/refs/heads/main/authentication/yuhu-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Property Management
- PropTech
- Real Estate
- Multifamily
- Rental
- Leasing
- Payments
- Partners API
---
