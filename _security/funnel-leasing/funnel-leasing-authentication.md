---
api_key_in:
- basic-auth-username
- authorization-header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Funnel Leasing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Funnel Leasing secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Funnel Leasing
provider_slug: funnel-leasing
scheme_count: 2
schemes:
- applies_to:
  - Customer API
  - Partner API
  description: 'HTTP Basic Authentication. The username is your API key and the password is blank. Requests must be made over HTTPS.

    '
  example: 'curl --user YOUR_API_KEY: https://api.funnelleasing.com/api/v2/onlineleasing-link/'
  name: basicAuth
  scheme: basic
  sources:
  - https://developer.funnelleasing.com/apis/customer-api/authentication
  type: http
- applies_to:
  - Partner API
  description: 'Partner API also supports supplying the API key as a Bearer token in the Authorization header.

    '
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.funnelleasing.com/apis/partner-api
  type: http
slug: funnel-leasing-authentication
source_filename: funnel-leasing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.funnelleasing.com/apis/customer-api/authentication\ndocs: https://developer.funnelleasing.com/apis/customer-api/authentication\nsummary:\n  types: [http]\n  http_schemes: [basic, bearer]\n  api_key_in: [basic-auth-username, authorization-header]\n  oauth2_flows: []\n  transport: HTTPS required\nnotes: >\n  Funnel issues API keys scoped to a customer account. Two key kinds exist:\n  public keys for client-side integrations and private keys for server-to-server\n  calls (private keys must be kept secret / stored in a secrets manager). The\n  Customer API authenticates with HTTP Basic where the username is the API key\n  and the password is left blank. The Partner API additionally accepts the API\n  key as a Bearer token in the Authorization header.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >\n      HTTP Basic Authentication. The username is your API key and the password\n\
  \      is blank. Requests must be made over HTTPS.\n    example: 'curl --user YOUR_API_KEY: https://api.funnelleasing.com/api/v2/onlineleasing-link/'\n    applies_to: [Customer API, Partner API]\n    sources: [https://developer.funnelleasing.com/apis/customer-api/authentication]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >\n      Partner API also supports supplying the API key as a Bearer token in the\n      Authorization header.\n    applies_to: [Partner API]\n    sources: [https://developer.funnelleasing.com/apis/partner-api]\nkey_types:\n  - kind: public\n    use: client-side integrations\n  - kind: private\n    use: server-to-server integrations; must be kept secret\nauth_responses:\n  - status: 200\n    meaning: OK — authenticated\n  - status: 401\n    meaning: Unauthorized — missing or invalid credentials\n  - status: 403\n    meaning: Forbidden — valid credentials but no access permission\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funnel-leasing/refs/heads/main/authentication/funnel-leasing-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Real Estate
- PropTech
- Property Management
- Multifamily
- Leasing
- CRM
- Webhooks
---
