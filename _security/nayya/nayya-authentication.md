---
api_key_in: []
api_specs:
- filename: nayya-accounts-openapi.json
  format: json
  label: Nayya Accounts API
  slug: nayya-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-accounts-openapi.json
- filename: nayya-benefits-openapi.json
  format: json
  label: Nayya Benefits API
  slug: nayya-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-benefits-openapi.json
- filename: nayya-choose-openapi.json
  format: json
  label: Nayya Choose API
  slug: nayya-choose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-choose-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nayya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nayya secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nayya
provider_slug: nayya
scheme_count: 1
schemes:
- description: JWT token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nayya-accounts-openapi.json
  - openapi/nayya-benefits-openapi.json
  - openapi/nayya-choose-openapi.json
  type: http
slug: nayya-authentication
source_filename: nayya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nayya-accounts-openapi.json, openapi/nayya-benefits-openapi.json, openapi/nayya-choose-openapi.json\ndocs: https://docs.nayya.com/docs/requesting-an-access-token-for-the-partners-api\nsummary:\n  types:\n  - http\n  token_flow: client-credentials\nsummary_notes: >-\n  Nayya Integrate uses a bearer-token model. Partners are issued a clientId and\n  clientSecret (delivered via a 1Password vault). Those credentials are exchanged\n  at POST /token (Accounts API) for a short-lived JWT accessToken with an expiresAt\n  timestamp. The JWT is then sent as `Authorization: Bearer <accessToken>` on every\n  API call. No OAuth2 scopes are declared in the specs; authorization is scoped to\n  the organization that owns the employer.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: JWT token\n  sources:\n  - openapi/nayya-accounts-openapi.json\n  - openapi/nayya-benefits-openapi.json\n  - openapi/nayya-choose-openapi.json\n\
  token_endpoint:\n  operation: get-token\n  method: POST\n  path: /token\n  server: https://integrate.nayya.com/accounts\n  request:\n    clientId: string\n    clientSecret: string\n  response:\n    accessToken: JWT string\n    expiresAt: expiration epoch time\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/authentication/nayya-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Employee Benefits
- Insurance
- Insurtech
- Health
- Decision Support
- HR Tech
- Enrollment
- Recommendations
- Artificial Intelligence
---
