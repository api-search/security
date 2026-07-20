---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Goget Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoGet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoGet
provider_slug: goget
scheme_count: 1
schemes:
- description: 'Account-level bearer token. Sent on every request alongside Accept: application/json and Content-Type: application/json headers.'
  format: Token token=<Your_Auth_Token>
  in: header
  name: TokenAuth
  parameter: Authorization
  source: https://api-docs.goget.my/
  type: apiKey
slug: goget-authentication
source_filename: goget-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api-docs.goget.my/\ndocs: https://api-docs.goget.my/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    GoGet uses a static account API token passed in the Authorization header\n    using the Rails-style \"Token token=<token>\" scheme. The token is generated\n    from the Business Account dashboard at https://web.goget.my/api after\n    upgrading to a Business Account. There is no OAuth2 authorization server and\n    no scope surface, so no scopes/ artifact is produced.\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token token=<Your_Auth_Token>'\n  description: >-\n    Account-level bearer token. Sent on every request alongside\n    Accept: application/json and Content-Type: application/json headers.\n  source: https://api-docs.goget.my/\ntoken_management:\n  generate_url: https://web.goget.my/api\n  requires: Business\
  \ Account\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goget/refs/heads/main/authentication/goget-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Delivery
- Logistics
- On-Demand
- Gig Economy
- Workforce
- Dispatch
- Malaysia
- Webhooks
---
