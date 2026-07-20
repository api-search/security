---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Dwolla Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Dwolla secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Dwolla
provider_slug: dwolla
scheme_count: 1
schemes:
- api_request_auth: 'Authorization: Bearer {access_token}'
  description: Application authorization (2-legged OAuth). The application exchanges its client_id and client_secret for an application access token that acts on the app's own behalf.
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  token_lifetime: 3600s (one hour); no refresh token — re-exchange credentials on expiry
  token_request_auth: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret)'
  token_urls:
    production: https://api.dwolla.com/token
    sandbox: https://api-sandbox.dwolla.com/token
  type: oauth2
slug: dwolla-authentication
source_filename: dwolla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.dwolla.com/docs/api-reference/api-fundamentals/making-requests-and-authentication\ndocs: https://developers.dwolla.com/docs/api-reference/api-fundamentals/making-requests-and-authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_delivery: bearer\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Application authorization (2-legged OAuth). The application exchanges its client_id and\n    client_secret for an application access token that acts on the app's own behalf.\n  token_urls:\n    production: https://api.dwolla.com/token\n    sandbox: https://api-sandbox.dwolla.com/token\n  grant_type: client_credentials\n  token_request_auth: \"HTTP Basic — Authorization: Basic base64(client_id:client_secret)\"\n  token_lifetime: \"3600s (one hour); no refresh token — re-exchange credentials on expiry\"\n  api_request_auth:\
  \ \"Authorization: Bearer {access_token}\"\nrequest_headers:\n  Accept: application/vnd.dwolla.v1.hal+json\n  Content-Type: application/vnd.dwolla.v1.hal+json (or application/json)\nscopes:\n  note: >-\n    The client-credentials application flow does not use scopes. Scope errors (InvalidScopes) can be\n    returned for endpoints requiring specific granted permissions; a public scope reference was not\n    located, so no scopes/ artifact is emitted (see errors/dwolla-problem-types.yml InvalidScopes).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/authentication/dwolla-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Payments
- ACH
- Bank Transfers
- Fintech
- Account-to-Account Payments
- Money Movement
- Instant Payments
- Open Banking
- Webhooks
- KYC
---
