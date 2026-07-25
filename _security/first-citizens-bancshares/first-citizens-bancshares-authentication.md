---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: First Citizens Bancshares Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: First Citizens BancShares secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: First Citizens BancShares
provider_slug: first-citizens-bancshares
scheme_count: 2
schemes:
- description: 'Client-credentials grant. Partners POST their registered client_id and client_secret to /v1/security/oauth/token and receive a short-lived bearer access token presented as `Authorization: Bearer <token>` on every subsequent call. This is the entry point for all commercial banking APIs.'
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://developer.svb.com/apis/commercial-banking-apis/authorization-api/1.0/authorization
  tokenUrl: https://api.svb.com/v1/security/oauth/token
  token_type: Bearer
  type: oauth2
- description: Detached JWS request signing. Each request body is signed with the partner's registered signing key; the compact detached signature is sent in the x-jws-signature header. Provides payload integrity and non-repudiation on top of the bearer token.
  format: detached-jws
  header: x-jws-signature
  name: JWSRequestSignature
  scheme: signature
  sources:
  - https://developer.svb.com/apis/commercial-banking-apis/authorization-api/1.0/json-web-signature-jws
  type: http
slug: first-citizens-bancshares-authentication
source_filename: first-citizens-bancshares-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.svb.com/apis/commercial-banking-apis/authorization-api/1.0/authorization\ndocs:\n  - https://developer.svb.com/apis/commercial-banking-apis/authorization-api/1.0/authorization\n  - https://developer.svb.com/apis/commercial-banking-apis/authorization-api/1.0/json-web-signature-jws\nnotes: >-\n  The SVB commercial banking platform (now part of First Citizens) uses a\n  two-layer security model documented on the Authorization API and JWS pages.\n  Layer 1 is OAuth 2.0 client-credentials: a partner exchanges its registered\n  client_id/client_secret at the token endpoint for a short-lived bearer access\n  token. Layer 2 is per-request message signing: the partner signs each request\n  payload with a registered private key and attaches a detached JSON Web\n  Signature (RFC 7515), Open-Banking style, so the server can verify integrity\n  and non-repudiation independent of transport. No OpenAPI securityScheme could\n\
  \  be derived because the machine-readable spec is partner-gated (api.svb.com\n  returns 401 anonymously); this profile is captured from the public docs.\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  message_signing: jws-detached          # RFC 7515, x-jws-signature header\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://api.svb.com/v1/security/oauth/token\n    token_type: Bearer\n    description: >-\n      Client-credentials grant. Partners POST their registered client_id and\n      client_secret to /v1/security/oauth/token and receive a short-lived\n      bearer access token presented as `Authorization: Bearer <token>` on every\n      subsequent call. This is the entry point for all commercial banking APIs.\n    sources:\n      - https://developer.svb.com/apis/commercial-banking-apis/authorization-api/1.0/authorization\n  - name: JWSRequestSignature\n    type: http\n    scheme:\
  \ signature\n    header: x-jws-signature\n    format: detached-jws                  # RFC 7515 detached JSON Web Signature\n    description: >-\n      Detached JWS request signing. Each request body is signed with the\n      partner's registered signing key; the compact detached signature is sent\n      in the x-jws-signature header. Provides payload integrity and\n      non-repudiation on top of the bearer token.\n    sources:\n      - https://developer.svb.com/apis/commercial-banking-apis/authorization-api/1.0/json-web-signature-jws\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-citizens-bancshares/refs/heads/main/authentication/first-citizens-bancshares-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Banking
- Financial Services
- Commercial Banking
- Payments
- ACH
- Wire Transfers
- Virtual Cards
- Open Banking
- Trust
- Investment
- Insurance
- United States
- Super Regional
---
