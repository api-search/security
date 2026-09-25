---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zenledger-authentication-api-openapi.yml
  format: yaml
  label: ZenLedger Authentication API
  slug: zenledger-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-authentication-api-openapi.yml
- filename: zenledger-companies-api-openapi.yml
  format: yaml
  label: ZenLedger Companies API
  slug: zenledger-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-companies-api-openapi.yml
- filename: zenledger-holdings-api-openapi.yml
  format: yaml
  label: ZenLedger Holdings API
  slug: zenledger-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-holdings-api-openapi.yml
- filename: zenledger-imports-api-openapi.yml
  format: yaml
  label: ZenLedger Imports API
  slug: zenledger-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-imports-api-openapi.yml
- filename: zenledger-polymarkets-api-openapi.yml
  format: yaml
  label: ZenLedger Polymarkets API
  slug: zenledger-polymarkets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-polymarkets-api-openapi.yml
- filename: zenledger-portfolios-api-openapi.yml
  format: yaml
  label: ZenLedger Portfolios API
  slug: zenledger-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-portfolios-api-openapi.yml
- filename: zenledger-supported-chains-api-openapi.yml
  format: yaml
  label: ZenLedger Supported Chains API
  slug: zenledger-supported-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-supported-chains-api-openapi.yml
- filename: zenledger-supported-currencies-api-openapi.yml
  format: yaml
  label: ZenLedger Supported Currencies API
  slug: zenledger-supported-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-supported-currencies-api-openapi.yml
- filename: zenledger-supported-exchanges-and-wallets-api-openapi.yml
  format: yaml
  label: ZenLedger Supported Exchanges and Wallets API
  slug: zenledger-supported-exchanges-and-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-supported-exchanges-and-wallets-api-openapi.yml
- filename: zenledger-taxes-api-openapi.yml
  format: yaml
  label: ZenLedger Taxes API
  slug: zenledger-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-taxes-api-openapi.yml
- filename: zenledger-transactions-api-openapi.yml
  format: yaml
  label: ZenLedger Transactions API
  slug: zenledger-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-transactions-api-openapi.yml
- filename: zenledger-users-api-openapi.yml
  format: yaml
  label: ZenLedger Users API
  slug: zenledger-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-users-api-openapi.yml
- filename: zenledger-wallet-screening-api-openapi.yml
  format: yaml
  label: ZenLedger Wallet Screening API
  slug: zenledger-wallet-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-wallet-screening-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zenledger Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZenLedger secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ZenLedger
provider_slug: zenledger
scheme_count: 2
schemes:
- content_type: application/json
  description: POST /oauth/token with a JSON body carrying client_id, client_secret and grant_type=client_credentials. A 200 returns access_token, token_type "Bearer", expires_in 1800 and scope "public". A 401 returns error / error_description for an invalid client; a 400 for a malformed request. The same endpoint is used to refresh after expiry — there is no refresh_token grant.
  flow: clientCredentials
  name: oauth2ClientCredentials
  request_body: '{"client_id": "...", "client_secret": "...", "grant_type": "client_credentials"}'
  response_fields:
  - access_token
  - token_type
  - expires_in
  - scope
  - created_at
  scopes_returned:
  - public
  source: https://docs.zenledger.io/compliance/v3/README.md
  token_url: https://api.zenledger.io/oauth/token
  type: oauth2
- bearerFormat: JWT
  description: 'Every non-token operation on both APIs requires the JWT in the Authorization header. Presenting an expired token returns error code ZENCS-AUTHGET-AA4 (Compliance) / ZENAGG-AUTHGET-AA4 (Aggregator) — "Invalid OAuth token: Need to refresh the token every 30 minutes".'
  header: 'Authorization: Bearer {jwt_token}'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zenledger-compliance-api-openapi.yml
  - openapi/zenledger-aggregator-api-openapi.yml
  type: http
slug: zenledger-authentication
source_filename: zenledger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.zenledger.io/compliance/v3/README.md\ndocs: https://docs.zenledger.io/compliance/v3/README.md\nsummary:\n  types:\n  - oauth2\n  - http\n  model: >-\n    One OAuth 2.0 client_credentials token endpoint fronts both published ZenLedger APIs. Credentials are issued by\n    ZenLedger out of band (there is no self-serve developer key). The resulting JWT is presented as an HTTP bearer\n    token on every other request and expires after 30 minutes. The wallet/exchange import endpoints add a second\n    layer: an HMAC-SHA256 request signature plus an AES-256-CBC encrypted request body.\ntoken_endpoint: https://api.zenledger.io/oauth/token\ntoken_lifetime_seconds: 1800\ncredential_issuance: assigned-by-provider\nself_serve_keys: false\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.zenledger.io/oauth/token\n  request_body: '{\"client_id\": \"...\", \"client_secret\"\
  : \"...\", \"grant_type\": \"client_credentials\"}'\n  content_type: application/json\n  response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  - scope\n  - created_at\n  scopes_returned:\n  - public\n  description: >-\n    POST /oauth/token with a JSON body carrying client_id, client_secret and grant_type=client_credentials. A 200\n    returns access_token, token_type \"Bearer\", expires_in 1800 and scope \"public\". A 401 returns error /\n    error_description for an invalid client; a 400 for a malformed request. The same endpoint is used to refresh\n    after expiry — there is no refresh_token grant.\n  source: https://docs.zenledger.io/compliance/v3/README.md\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer {jwt_token}'\n  description: >-\n    Every non-token operation on both APIs requires the JWT in the Authorization header. Presenting an expired token\n    returns error code ZENCS-AUTHGET-AA4 (Compliance) /\
  \ ZENAGG-AUTHGET-AA4 (Aggregator) — \"Invalid OAuth token: Need\n    to refresh the token every 30 minutes\".\n  sources:\n  - openapi/zenledger-compliance-api-openapi.yml\n  - openapi/zenledger-aggregator-api-openapi.yml\nrequest_signing:\n  applies_to:\n  - POST /compliance/api/v3/companies/{company_reference}/users/{user_id}/imports\n  - POST /compliance/api/v1/companies/{company_reference}/users/{user_id}/imports\n  signature:\n    header: X-Signature\n    algorithm: HMAC-SHA256\n    encoding: hex\n    signed_material: >-\n      The published TypeScript example computes the HMAC over the base64 ciphertext of the encrypted payload using\n      the shared API secret. The prose above the example describes concatenating method, URL path, query parameters\n      and body before hashing; the two descriptions differ and the code sample is the operative one.\n  encryption:\n    algorithm: AES-256-CBC\n    key_derivation: SHA-256 digest of the shared secret\n    iv: 16 random bytes, sent base64-encoded\
  \ in the request body as `iv`\n    envelope_fields:\n    - data\n    - iv\n    - signature\n  key_exchange: The encryption key is shared out of band between client and ZenLedger.\n  source: https://docs.zenledger.io/compliance/v3/README.md\nlive_probe:\n  date: '2026-09-05'\n  probes:\n  - url: https://api.zenledger.io/oauth/token\n    method: POST\n    body: '{\"grant_type\":\"client_credentials\"}'\n    credentials_sent: false\n    http_status: 401\n    response: '{\"error\":\"invalid_client\",\"error_description\":\"Client authentication failed due to unknown client, no client authentication included, or unsupported authentication method.\"}'\n  - url: https://api.zenledger.io/compliance/api/v3/chains\n    method: GET\n    credentials_sent: false\n    http_status: 401\n  finding: >-\n    Both APIs are live at the documented host and enforce authentication. The token endpoint returns a conformant\n    RFC 6749 error object; a protected reference-data endpoint returns 401 to an anonymous\
  \ caller. Confirmed\n    anonymously — no credentials were used and no protected data was read.\n\nnotes:\n- The OpenAPI documents in this repo model the bearer scheme only, because that is what the Postman collection\n  encodes per request; the OAuth 2.0 token flow is documented in prose in the collection's Authentication folder and\n  is captured here.\n- Scope is returned as the single literal value \"public\"; ZenLedger publishes no scope reference page and no\n  per-scope authorization model, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/authentication/zenledger-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Crypto Tax
- Digital Assets
- Tax Compliance
- Blockchain Analytics
- RegTech
- Accounting
- Sanctions Screening
- Financial Services
- Portfolio Aggregation
- Cryptocurrency
---
