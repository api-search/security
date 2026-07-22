---
api_key_in: []
api_specs:
- filename: mvmnt-openapi-original.yml
  format: yaml
  label: MVMNT API
  slug: mvmnt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mvmnt/refs/heads/main/openapi/mvmnt-openapi-original.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mvmnt Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: MVMNT secures its APIs with oauth2 and http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: MVMNT
provider_slug: mvmnt
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained via the client-credentials flow at https://api.mvmnt.io/oauth2/token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/mvmnt-openapi-original.yml
  type: http
slug: mvmnt-authentication
source_filename: mvmnt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mvmnt.io/getting-started/authentication\nspec_source: openapi/mvmnt-openapi-original.yml\ndocs: https://docs.mvmnt.io/getting-started/authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\nmodel:\n  flow: oauth2-client-credentials\n  token_endpoint: https://api.mvmnt.io/oauth2/token\n  token_type: Bearer\n  token_format: JWT\n  token_lifetime_seconds: 3600\n  scope: mvmnt-api\n  request_header: 'Authorization: Bearer <access_token>'\n  credentials: Client ID + Client Secret, provisioned by an MVMNT account manager.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained via the client-credentials flow at https://api.mvmnt.io/oauth2/token\n  sources:\n  - openapi/mvmnt-openapi-original.yml\nwebhook_auth:\n  header: x-api-key\n  note: Inbound webhook deliveries carry an x-api-key header holding the\
  \ webhook token configured in the MVMNT UI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mvmnt/refs/heads/main/authentication/mvmnt-authentication.yml
summary_line: oauth2/http · 1 scheme
tags:
- Freight
- Logistics
- Transportation Management System
- Supply Chain
- Brokerage
- Shipping
- Payments
- Company
---
