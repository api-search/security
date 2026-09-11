---
anonymous_access: false
api_key_in:
- body
api_specs:
- filename: aeropay-v2-openapi.yml
  format: yaml
  label: Aeropay v2 API
  slug: aeropay-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-v2-openapi.yml
auth_types:
- http-bearer
- credentials-exchange
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aeropay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aeropay secures its APIs with http-bearer and credentials-exchange across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aeropay
provider_slug: aeropay
scheme_count: 2
schemes:
- applies_to: 31 of 32 operations (every operation except POST /v2/token)
  bearer_format: JWT
  description: A transient JSON Web Token minted by POST /v2/token. Tokens expire 30 minutes after issue and must be re-requested; there is no refresh-token flow.
  format: Bearer {{token}}
  in: header
  name: AeropayBearerToken
  parameter: authorization
  scheme: bearer
  source: https://dev.aero.inc/reference/post_v2-token
  ttl: 30 minutes
  type: http
- applies_to: POST /v2/token only
  description: Merchant API key and secret plus a numeric merchant id are POSTed as a JSON body to /v2/token in exchange for a bearer token. Keys are environment-specific — a sandbox key will not authenticate against production (error AP002).
  environments_separate: true
  in: request-body
  name: AeropayApiCredentials
  parameters:
  - apiKey
  - apiSecret
  - id
  - scope
  - userId
  source: https://dev.aero.inc/docs/token-scopes
  type: credentials-exchange
slug: aeropay-authentication
source_filename: aeropay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: openapi/aeropay-v2-openapi.yml\ndocs: https://dev.aero.inc/docs/token-scopes\ndocs_additional:\n- https://dev.aero.inc/reference/post_v2-token\n- https://dev.aero.inc/docs/standard-transaction-step-1-authentication\n- https://dev.aero.inc/docs/oauth-connections\nspec_gap: 'The published OpenAPI 3.0.0 document declares components.securitySchemes as an EMPTY object\n  and sets no root-level or operation-level security[]. Authentication is expressed only as a plain\n  `authorization` header parameter on 31 of the 32 operations, so no machine reading the contract alone\n  can discover the auth model. Everything below is read from the prose documentation, which is why this\n  artifact is method: searched rather than derived — derive-authentication.py returns zero schemes.'\nsummary:\n  types:\n  - http-bearer\n  - credentials-exchange\n  api_key_in:\n  - body\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n\
  - name: AeropayBearerToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  parameter: authorization\n  format: 'Bearer {{token}}'\n  applies_to: 31 of 32 operations (every operation except POST /v2/token)\n  ttl: 30 minutes\n  source: https://dev.aero.inc/reference/post_v2-token\n  description: 'A transient JSON Web Token minted by POST /v2/token. Tokens expire 30 minutes after\n    issue and must be re-requested; there is no refresh-token flow.'\n- name: AeropayApiCredentials\n  type: credentials-exchange\n  in: request-body\n  parameters:\n  - apiKey\n  - apiSecret\n  - id\n  - scope\n  - userId\n  applies_to: POST /v2/token only\n  environments_separate: true\n  source: https://dev.aero.inc/docs/token-scopes\n  description: 'Merchant API key and secret plus a numeric merchant id are POSTed as a JSON body to\n    /v2/token in exchange for a bearer token. Keys are environment-specific — a sandbox key will not\n    authenticate against production (error AP002).'\n\
  token_scopes:\n  model: 'Aeropay calls these \"scopes\" but they are NOT OAuth 2.0 scopes — there is no authorization\n    server, no consent step and no scope string on a token request beyond a single enum. The `scope`\n    body parameter selects WHICH ACTOR the token represents, and each operation requires one specific\n    actor. No scopes/ artifact is emitted for this provider because there is no OAuth surface to\n    describe; the actor model is recorded here instead.'\n  docs: https://dev.aero.inc/docs/token-scopes\n  scopes:\n  - scope: merchant\n    required_parameters:\n    - apiKey\n    - apiSecret\n    - scope\n    - id\n    description: Acts on behalf of the merchant organisation.\n    example_operations:\n    - POST /v2/user\n    - POST /v2/transactionSearch\n    - POST /v2/payoutTransaction\n    - GET /v2/merchant/tipConfiguration\n  - scope: userForMerchant\n    required_parameters:\n    - apiKey\n    - apiSecret\n    - scope\n    - id\n    - userId\n    description: Acts\
  \ on behalf of one Aeropay user created by that merchant.\n    example_operations:\n    - GET /v2/user\n    - GET /v2/bankAccounts\n    - GET /v2/aggregatorCredentials\n    - POST /v2/transaction\n    - POST /v2/preauthTransaction\nend_user_bank_authorization:\n  mechanism: 'Separate from API authentication. End users authorise access to their own bank account\n    through the Aerosync widget, which Aeropay describes as OAuth-first bank linking. The integrator\n    calls GET /v2/aggregatorCredentials to mint a one-time widget URL and token, the user completes the\n    bank''s own OAuth or credential flow inside the widget, and the returned connectionId is attached\n    with POST /v2/linkAccountFromAggregator.'\n  docs: https://dev.aero.inc/docs/oauth-connections\nauth_errors:\n  source: https://dev.aero.inc/docs/error-handling\n  note: 'Authentication failures are returned with an HTTP 200 body carrying an error object, not an HTTP\n    401, for most codes. See errors/aeropay-error-codes.yml.'\n\
  \  codes:\n  - code: AP001\n    meaning: API key and secret key required.\n  - code: AP002\n    meaning: Invalid API key or secret key, or wrong environment.\n  - code: AP003\n    meaning: Merchant account locked.\n  - code: AP004\n    meaning: Missing authorization header token.\n  - code: AP006\n    meaning: Client is not authorized for this scope.\n  - code: AP007\n    meaning: Token has expired.\n  - code: AP008\n    meaning: Invalid token.\n  - code: AP101\n    meaning: No authenticated user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/authentication/aeropay-authentication.yml
summary_line: http-bearer/credentials-exchange · 2 schemes
tags:
- Payments
- Pay by bank
- ACH
- Open Banking
- Fintech
- Bank linking
- Financial Services
- Real-time payments
- Webhook
- Payouts
- MCP
- Risk & fraud
---
