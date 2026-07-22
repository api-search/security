---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Solaris Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Solaris secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Solaris
provider_slug: solaris
scheme_count: 1
schemes:
- description: 'Solaris uses OAuth2 client-credentials. Base64-encode "client_id:client_secret" and send it as an HTTP Basic Authorization header to the token endpoint with grant_type=client_credentials and scope=partners. The endpoint returns a short-lived (1 hour / 3600s) bearer access_token that must be sent as "Authorization: Bearer {token}" on every subsequent API request. A 401 Unauthorized indicates an expired or malformed token; the client must fetch a new token and retry.'
  flows:
  - flow: clientCredentials
    grant_type: client_credentials
    scopes:
      partners: Standard API access scope required for partner API calls.
    tokenUrl_production: https://auth.solarisbank.de/oauth2/token
    tokenUrl_sandbox: https://auth.solaris-sandbox.de/oauth2/token
  name: OAuth2
  sources:
  - https://docs.solarisgroup.com/api-reference/authentication
  type: oauth2
slug: solaris-authentication
source_filename: solaris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.solarisgroup.com/api-reference/authentication\ndocs: https://docs.solarisgroup.com/api-reference/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: bearer\n  token_ttl_seconds: 3600\n  credential_transport: http-basic-base64\nschemes:\n  - name: OAuth2\n    type: oauth2\n    description: >-\n      Solaris uses OAuth2 client-credentials. Base64-encode\n      \"client_id:client_secret\" and send it as an HTTP Basic Authorization\n      header to the token endpoint with grant_type=client_credentials and\n      scope=partners. The endpoint returns a short-lived (1 hour / 3600s)\n      bearer access_token that must be sent as \"Authorization: Bearer {token}\"\n      on every subsequent API request. A 401 Unauthorized indicates an expired\n      or malformed token; the client must fetch a new token and retry.\n    flows:\n      - flow: clientCredentials\n        tokenUrl_sandbox:\
  \ https://auth.solaris-sandbox.de/oauth2/token\n        tokenUrl_production: https://auth.solarisbank.de/oauth2/token\n        grant_type: client_credentials\n        scopes:\n          partners: Standard API access scope required for partner API calls.\n    sources: [https://docs.solarisgroup.com/api-reference/authentication]\npermissions_model: >-\n  Beyond the OAuth scope, per-endpoint access is governed by policies granted\n  to each partner by their Solaris Partner Manager based on the products they\n  implement (a token only unlocks the API actions the partner is permitted to\n  use).\nlegacy:\n  endpoint: POST /oauth/token\n  status: deprecated\n  note: >-\n    The legacy /oauth/token endpoint (JSON client_id/client_secret body) is\n    deprecated; new integrations must use the OAuth2 token endpoints above.\ncustomer_authentication:\n  - name: Device binding\n    detail: Links a physical device to a customer account via SMS OTP or Activation Code (QR); prerequisite for SCA.\n  -\
  \ name: Strong Customer Authentication (SCA)\n    detail: PSD2-mandated two-factor authorization for sensitive actions across the EEA.\n  - name: 3D Secure (3DS)\n    detail: Extra authentication layer for online card payments via SMS OTP or in-app notification.\n  - name: PSD2 SCA flow (TPP)\n    detail: Split authentication where the partner handles 1FA and Solaris handles 2FA via OTP.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solaris/refs/heads/main/authentication/solaris-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Banking
- Banking as a Service
- Embedded Finance
- Payments
- SEPA
- Cards
- KYC
- Lending
- Compliance
- OAuth2
- Webhooks
- Germany
---
