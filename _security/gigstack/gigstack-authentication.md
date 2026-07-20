---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gigstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gigstack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gigstack
provider_slug: gigstack
scheme_count: 1
schemes:
- bearerFormat: JWT
  format: 'Authorization: Bearer <JWT_TOKEN>'
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs.gigstack.io
  token_source: https://app.gigstack.pro/settings?subtab=api
  type: http
slug: gigstack-authentication
source_filename: gigstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.gigstack.io/welcome-to-gigstack-api-1385870m0\ndocs: https://docs.gigstack.io/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    gigstack API v2 authenticates with a Bearer JWT token passed in the\n    Authorization header. Tokens are issued per team from the dashboard at\n    app.gigstack.pro/settings > API. There is no OAuth authorization-code\n    surface; the token is a long-lived API key presented as a bearer credential.\n    Test vs live is distinguished by the key itself (livemode flag on responses\n    and webhook events), not by a separate base URL.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    location: header\n    header: Authorization\n    format: 'Authorization: Bearer <JWT_TOKEN>'\n    token_source: https://app.gigstack.pro/settings?subtab=api\n    sources: [docs.gigstack.io]\n\
  multi_team:\n  parameter: team\n  description: >-\n    Requests may target a specific team via a `team` parameter, allowing a\n    single token holder to manage resources across multiple teams (gigstack\n    Connect / agency model).\nlegacy:\n  v1:\n    scheme: apiKey\n    header: X-API-Key\n    status: deprecated\n    note: >-\n      API v1 (https://gigstack-cfdi-bjekv7t4.uc.gateway.dev/v1) used an X-API-Key\n      header. v2 replaces this with Authorization: Bearer JWT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigstack/refs/heads/main/authentication/gigstack-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Invoicing
- CFDI
- SAT
- Tax Compliance
- Payments
- Billing
- Collections
- Mexico
- Accounts Receivable
---
