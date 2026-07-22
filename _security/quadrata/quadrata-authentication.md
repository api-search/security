---
api_key_in:
- header
auth_types:
- apiKey
- http-basic
- ecdsa-request-signature
- jwt-access-token
description: ''
kind: authentication
layout: security
method: searched
name: Quadrata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quadrata secures its APIs with apiKey, http-basic, ecdsa-request-signature, and jwt-access-token across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Quadrata
provider_slug: quadrata
scheme_count: 4
schemes:
- endpoints:
    integration: https://int.quadrata.com/api/v1/login
    production: https://prod.quadrata.com/api/v1/login
  flow: 'POST /api/v1/login with {"apiKey": "<COMPANY_API_KEY>"} returns a JWT accessToken (type: login, 60-minute expiry) used to initialize the client onboarding SDK (<QuadClient>).'
  in: body
  name: LoginApiKey
  parameter: apiKey
  type: apiKey
- format: Basic {base64(API_KEY)}
  header: Authorization
  in: header
  name: BasicApiKey
  notes: Same company API_KEY, base64-encoded, on all server-side privacy/screening endpoints.
  scheme: basic
  type: http
- algorithm: ECDSA
  auto_generated_by_sdk: true
  header: Signature
  in: header
  key_pair: Integrator generates an ECDSA key pair; the private signing key never leaves the integrator and is never known to Quadrata; the public key is registered with Quadrata to map the API Login Key.
  name: EcdsaRequestSignature
  signing_message:
    encoding: base64-url
    join: newline
    lifetime_seconds: 15
    nonce: appended to the signature delimited by '.', also base64-url encoded
    parts:
    - method (uppercase)
    - absolute path
    - query string (no '?')
    - HTTP Date header
    - nonce (optional)
  type: signature
- format: base64(authToken:accessToken)
  header: X-Access-Token
  in: header
  name: PrivacyAccessToken
  notes: One-time-use token obtained from GET /api/v1/privacy/access/{wallet}; required (in addition to Basic auth + Signature) to fetch consented privacy (PII) data. Reuse returns 401 Unauthorized.
  type: one-time-token
slug: quadrata-authentication
source_filename: quadrata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.quadrata.com/integration/how-to-integrate/request-privacy-data/api-requests/how-to-sign-api\ndocs: https://docs.quadrata.com/integration/how-to-integrate/onboard-users/individual-passport-onboarding/2.-api-authentication\nsummary:\n  types: [apiKey, http-basic, ecdsa-request-signature, jwt-access-token]\n  api_key_in: [header]\n  notes: >-\n    Quadrata uses a company API_KEY. Client onboarding flows exchange the API_KEY at POST /api/v1/login\n    for a short-lived (60 minute) JWT accessToken passed to the client SDK. Server-only endpoints (privacy\n    data, wallet screening) authenticate with HTTP Basic (base64 of the API_KEY) plus an ECDSA request\n    signature over method+path+query+Date(+nonce), verified against a public signing key registered with\n    Quadrata. Signatures have a 15-second lifetime.\nschemes:\n- name: LoginApiKey\n  type: apiKey\n  in: body\n  parameter: apiKey\n  flow: >-\n    POST /api/v1/login\
  \ with {\"apiKey\": \"<COMPANY_API_KEY>\"} returns a JWT accessToken (type: login,\n    60-minute expiry) used to initialize the client onboarding SDK (<QuadClient>).\n  endpoints:\n    production: https://prod.quadrata.com/api/v1/login\n    integration: https://int.quadrata.com/api/v1/login\n- name: BasicApiKey\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  format: 'Basic {base64(API_KEY)}'\n  notes: Same company API_KEY, base64-encoded, on all server-side privacy/screening endpoints.\n- name: EcdsaRequestSignature\n  type: signature\n  algorithm: ECDSA\n  in: header\n  header: Signature\n  key_pair: >-\n    Integrator generates an ECDSA key pair; the private signing key never leaves the integrator and is\n    never known to Quadrata; the public key is registered with Quadrata to map the API Login Key.\n  signing_message:\n    parts:\n    - method (uppercase)\n    - absolute path\n    - query string (no '?')\n    - HTTP Date header\n    - nonce (optional)\n \
  \   join: newline\n    encoding: base64-url\n    nonce: appended to the signature delimited by '.', also base64-url encoded\n    lifetime_seconds: 15\n  auto_generated_by_sdk: true\n- name: PrivacyAccessToken\n  type: one-time-token\n  in: header\n  header: X-Access-Token\n  format: 'base64(authToken:accessToken)'\n  notes: >-\n    One-time-use token obtained from GET /api/v1/privacy/access/{wallet}; required (in addition to Basic\n    auth + Signature) to fetch consented privacy (PII) data. Reuse returns 401 Unauthorized.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quadrata/refs/heads/main/authentication/quadrata-authentication.yml
summary_line: apiKey/http-basic/ecdsa-request-signature/jwt-access-token · 4 schemes
tags:
- Company
- Crypto Web3
- Identity
- Digital Identity
- KYC
- KYB
- AML
- Compliance
- Wallet Screening
- Blockchain
- Web3
- Decentralized Identity
---
