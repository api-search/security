---
api_key_in: []
api_specs:
- filename: arch-labs-client-api-openapi.json
  format: json
  label: Arch Client API
  slug: arch-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch-labs/refs/heads/main/openapi/arch-labs-client-api-openapi.json
auth_types:
- http
description: 'The Arch Client API uses JWT bearer-token authentication. Credentials (a Client ID and Client Secret) are requested from Arch at api-support@arch.co. Clients exchange those for an access token via a POST to /client-api/v0/auth/token with a JSON body {clientId, clientSecret}. The returned JWT is sent on subsequent requests as `authorization: Bearer <token>` and should be stored and reused until it expires (the exp claim in the decoded JWT is the Unix-epoch expiry). All other endpoints require the BearerAuth scheme.'
kind: authentication
layout: security
method: searched
name: Arch Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arch Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arch Labs
provider_slug: arch-labs
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/arch-labs-client-api-openapi.json
  type: http
slug: arch-labs-authentication
source_filename: arch-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/arch-labs-client-api-openapi.json\ndocs: https://arch.co/client-api/api-docs/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_grant: client-credentials\ndescription: >-\n  The Arch Client API uses JWT bearer-token authentication. Credentials (a Client ID and Client Secret)\n  are requested from Arch at api-support@arch.co. Clients exchange those for an access token via a POST\n  to /client-api/v0/auth/token with a JSON body {clientId, clientSecret}. The returned JWT is sent on\n  subsequent requests as `authorization: Bearer <token>` and should be stored and reused until it\n  expires (the exp claim in the decoded JWT is the Unix-epoch expiry). All other endpoints require the\n  BearerAuth scheme.\ntoken_endpoint: POST https://arch.co/client-api/v0/auth/token\ntoken_format: JWT\nheader: 'authorization: Bearer <access_token>'\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ JWT\n  sources:\n  - openapi/arch-labs-client-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arch-labs/refs/heads/main/authentication/arch-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Alternative Investments
- Private Markets
- Wealth Management
- Investment Management
- Financial Services
- Data Aggregation
---
