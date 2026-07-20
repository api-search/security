---
api_key_in:
- header
api_specs:
- filename: lightspark-grid-openapi-original.yml
  format: yaml
  label: Grid API
  slug: grid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightspark/refs/heads/main/openapi/lightspark-grid-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lightspark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightspark secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lightspark
provider_slug: lightspark
scheme_count: 3
schemes:
- description: API token authentication using format `<api token id>:<api client secret>`
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/lightspark-grid-openapi-original.yml
  type: http
- description: 'Bearer token authentication for agent-scoped endpoints. The token is the `accessToken` returned when redeeming a device code via `POST /agents/device-codes/{code}/redeem`. Agent credentials are user-scoped: all requests are automatically bound to the agent''s associated customer and subject to the agent''s policy.'
  name: AgentAuth
  scheme: bearer
  sources:
  - openapi/lightspark-grid-openapi-original.yml
  type: http
- description: 'Secp256r1 (P-256) asymmetric signature of the webhook payload, which can be used to verify that the webhook was sent by Grid.

    To verify the signature:

    1. Get the Grid public key provided to you during integration

    2. Decode the base64 signature from the header

    3. Create a SHA-256 hash of the request body

    4. Verify the signature using the public key and the hash


    If the signature verification succee'
  in: header
  name: WebhookSignature
  parameter: X-Grid-Signature
  sources:
  - openapi/lightspark-grid-openapi-original.yml
  type: apiKey
slug: lightspark-authentication
source_filename: lightspark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lightspark-grid-openapi-original.yml\ndocs: https://docs.lightspark.com/api-reference/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    Grid has no OAuth2 authorization server and therefore no OAuth scope surface — scopes/ is\n    intentionally absent. Platform calls use HTTP Basic with the API token id as username and the\n    client secret as password; agent calls use a user-scoped bearer token. Tokens are scoped to\n    exactly one environment (production or sandbox). API tokens are managed through the API itself\n    via createToken / listTokens / getTokenById / deleteTokenById.\n  additional_signals:\n  - header: Grid-Wallet-Signature\n    description: >-\n      P-256 session-key signature over the exact `payloadToSign` returned by Grid. Required on\n      embedded-wallet actions — add/revoke credential, revoke session, wallet export, wallet\
  \ privacy\n      update, and quote execution from an embedded wallet. Paired with the Request-Id header.\n  - header: Request-Id\n    description: Replayed from the challenge response on signed-retry flows; format `Request:<uuid>`.\n  embedded_wallet_credential_types:\n  - EMAIL_OTP\n  - SMS_OTP\n  - PASSKEY\n  - OAUTH\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: API token authentication using format `<api token id>:<api client secret>`\n  sources:\n  - openapi/lightspark-grid-openapi-original.yml\n- name: AgentAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token authentication for agent-scoped endpoints. The token is the `accessToken`\n    returned when redeeming a device code via `POST /agents/device-codes/{code}/redeem`. Agent\n    credentials are user-scoped: all requests are automatically bound to the agent''s associated\n    customer and subject to the agent''s policy.'\n  sources:\n  - openapi/lightspark-grid-openapi-original.yml\n- name:\
  \ WebhookSignature\n  type: apiKey\n  in: header\n  parameter: X-Grid-Signature\n  description: |-\n    Secp256r1 (P-256) asymmetric signature of the webhook payload, which can be used to verify that the webhook was sent by Grid.\n    To verify the signature:\n    1. Get the Grid public key provided to you during integration\n    2. Decode the base64 signature from the header\n    3. Create a SHA-256 hash of the request body\n    4. Verify the signature using the public key and the hash\n\n    If the signature verification succee\n  sources:\n  - openapi/lightspark-grid-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightspark/refs/heads/main/authentication/lightspark-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Payments
- Cross-Border Payments
- Stablecoins
- Bitcoin
- Lightning Network
- Embedded Finance
- Agentic Payments
- Cards
- KYC
- Financial Services
- Foreign Exchange
---
