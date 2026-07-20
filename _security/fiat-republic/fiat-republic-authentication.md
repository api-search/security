---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fiat Republic Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Fiat Republic secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Fiat Republic
provider_slug: fiat-republic
scheme_count: 1
schemes:
- access_token_format: JWT (bearer)
  access_token_ttl_seconds: 3599
  applied_via: Authorization Bearer header on all protected endpoints
  credentials: URL-encoded form data (client_id, client_secret, grant_type, scope)
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  scopes:
  - PAYMENTS
  - OXYGEN
  sources:
  - https://docs.fiatrepublic.com/docs/authentication
  token_url_sandbox: https://sandbox.fiatrepublic.com/passport/oauth/token
  type: oauth2
slug: fiat-republic-authentication
source_filename: fiat-republic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fiatrepublic.com/docs/authentication\ndocs: https://docs.fiatrepublic.com/docs/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_transport: bearer\n  request_signing: none\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url_sandbox: https://sandbox.fiatrepublic.com/passport/oauth/token\n  grant_type: client_credentials\n  credentials: URL-encoded form data (client_id, client_secret, grant_type, scope)\n  scopes:\n  - PAYMENTS\n  - OXYGEN\n  access_token_format: JWT (bearer)\n  access_token_ttl_seconds: 3599\n  applied_via: Authorization Bearer header on all protected endpoints\n  sources: [https://docs.fiatrepublic.com/docs/authentication]\nnotes: >-\n  OAuth 2.0 client-credentials flow. Client id/secret are generated in the Developers section of\n  the Dashboard; the secret is shown once and cannot be retrieved afterward. A\
  \ separate PAYMENTS\n  vs OXYGEN scope selects which product surface the access token can reach (PAYMENTS expands to\n  \"PAYMENTS payments.*\"). No HMAC/request signing on API calls; webhooks are separately signed\n  with HMAC-SHA256 (see conventions/ and asyncapi/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiat-republic/refs/heads/main/authentication/fiat-republic-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Banking
- Payments
- Fintech
- Cryptocurrency
- Stablecoins
- Banking-as-a-Service
- Embedded Finance
- Compliance
- KYC
- SEPA
- Faster Payments
---
