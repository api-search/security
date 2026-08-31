---
api_key_in: []
api_specs:
- filename: interchecks-accounts-api-openapi.yml
  format: yaml
  label: Interchecks Accounts API
  slug: interchecks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-accounts-api-openapi.yml
- filename: interchecks-authentication-api-openapi.yml
  format: yaml
  label: Interchecks Authentication API
  slug: interchecks-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-authentication-api-openapi.yml
- filename: interchecks-oauth2-api-openapi.yml
  format: yaml
  label: Interchecks Oauth2 API
  slug: interchecks-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-oauth2-api-openapi.yml
- filename: interchecks-payers-api-openapi.yml
  format: yaml
  label: Interchecks Payers API
  slug: interchecks-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payers-api-openapi.yml
- filename: interchecks-payload-api-openapi.yml
  format: yaml
  label: Interchecks Payload API
  slug: interchecks-payload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payload-api-openapi.yml
- filename: interchecks-payment-accounts-bank-api-openapi.yml
  format: yaml
  label: Interchecks Payment Accounts - Bank API
  slug: interchecks-payment-accounts-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payment-accounts-bank-api-openapi.yml
- filename: interchecks-payment-accounts-card-api-openapi.yml
  format: yaml
  label: Interchecks Payment Accounts - Card API
  slug: interchecks-payment-accounts-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payment-accounts-card-api-openapi.yml
- filename: interchecks-payment-accounts-paypal-api-openapi.yml
  format: yaml
  label: Interchecks Payment Accounts - PayPal API
  slug: interchecks-payment-accounts-paypal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payment-accounts-paypal-api-openapi.yml
- filename: interchecks-payments-api-openapi.yml
  format: yaml
  label: Interchecks Payments API
  slug: interchecks-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payments-api-openapi.yml
- filename: interchecks-recipient-emails-api-openapi.yml
  format: yaml
  label: Interchecks Recipient Emails API
  slug: interchecks-recipient-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-recipient-emails-api-openapi.yml
- filename: interchecks-recipient-verification-api-openapi.yml
  format: yaml
  label: Interchecks Recipient Verification API
  slug: interchecks-recipient-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-recipient-verification-api-openapi.yml
- filename: interchecks-recipients-api-openapi.yml
  format: yaml
  label: Interchecks Recipients API
  slug: interchecks-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-recipients-api-openapi.yml
- filename: interchecks-reports-api-openapi.yml
  format: yaml
  label: Interchecks Reports API
  slug: interchecks-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-reports-api-openapi.yml
- filename: interchecks-test-harness-api-openapi.yml
  format: yaml
  label: Interchecks Test Harness API
  slug: interchecks-test-harness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-test-harness-api-openapi.yml
- filename: interchecks-transactions-api-openapi.yml
  format: yaml
  label: Interchecks Transactions API
  slug: interchecks-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-transactions-api-openapi.yml
- filename: interchecks-widgets-api-openapi.yml
  format: yaml
  label: Interchecks Widgets API
  slug: interchecks-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-widgets-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Interchecks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Interchecks secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Interchecks
provider_slug: interchecks
scheme_count: 2
schemes:
- client_authentication: HTTP Basic — Authorization header carrying base64(clientId:secret).
  flow: clientCredentials
  grant_type: client_credentials
  name: sec0
  operation_id: get-access-token
  request_content_type: application/x-www-form-urlencoded
  response_fields:
  - access_token
  - expires_in
  - token_type
  sandbox_token_endpoint: https://test.api.interchecks.io/api/v2/oauth2/token
  scopes: []
  scopes_note: The published securityScheme declares no scopes and the documentation defines no scope or permission vocabulary. Authorization is scoped by the payer_id in the request path and by the payer/aggregator configuration held by Interchecks, not by OAuth scopes. No scopes/ artifact is emitted for this provider.
  sources:
  - openapi/interchecks-payments-api-v2.json
  - https://docs-v2.interchecks.com/reference/get-access-token
  token_endpoint: https://prod.api.interchecks.io/api/v2/oauth2/token
  type: oauth2
- bearer_format: JWT
  name: httpBearer
  note: The older published document (payments-api-v2.json, OpenAPI 3.0.0) declares the same credential as a plain http/bearer scheme rather than an oauth2 clientCredentials flow.
  scheme: bearer
  sources:
  - openapi/interchecks-payments-api-v2-registry.json
  type: http
slug: interchecks-authentication
source_filename: interchecks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://docs-v2.interchecks.com/reference/get-access-token\ndocs: https://docs-v2.interchecks.com/docs/getting-started\nsummary:\n  types:\n  - oauth2\n  - http\n  model: >-\n    OAuth 2.0 client_credentials. The caller exchanges a client id and secret for a short-lived\n    JWT access token, then presents it as an HTTP Bearer token on every subsequent call. Keys and\n    secrets are self-managed by the payer/aggregator in the Interchecks Portal Developer area.\n  token_lifetime_seconds: 900\n  token_format: JWT\nschemes:\n- name: sec0\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://prod.api.interchecks.io/api/v2/oauth2/token\n  sandbox_token_endpoint: https://test.api.interchecks.io/api/v2/oauth2/token\n  operation_id: get-access-token\n  client_authentication: >-\n    HTTP Basic — Authorization header carrying base64(clientId:secret).\n  grant_type: client_credentials\n  request_content_type: application/x-www-form-urlencoded\n\
  \  response_fields:\n  - access_token\n  - expires_in\n  - token_type\n  scopes: []\n  scopes_note: >-\n    The published securityScheme declares no scopes and the documentation defines no scope or\n    permission vocabulary. Authorization is scoped by the payer_id in the request path and by the\n    payer/aggregator configuration held by Interchecks, not by OAuth scopes. No scopes/ artifact\n    is emitted for this provider.\n  sources:\n  - openapi/interchecks-payments-api-v2.json\n  - https://docs-v2.interchecks.com/reference/get-access-token\n- name: httpBearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  note: >-\n    The older published document (payments-api-v2.json, OpenAPI 3.0.0) declares the same\n    credential as a plain http/bearer scheme rather than an oauth2 clientCredentials flow.\n  sources:\n  - openapi/interchecks-payments-api-v2-registry.json\ntenancy:\n  path_parameter: payer_id\n  note: >-\n    Every business operation is addressed under /api/v2/{payer_id}/...,\
  \ where payer_id identifies\n    the aggregator or the payer. An aggregator-level API account acts across its payers.\nadditional_controls:\n- name: Payload envelope encryption\n  header: 'X-ENCRYPTED: <Payer ID>'\n  description: >-\n    Optional per-payer envelope encryption of request and response bodies. Payload is encrypted\n    with AES (AES/GCM/NoPadding by default, AES/CBC/PKCS5Padding via X-AES-MODE:\n    CBC_PKCS5PADDING); the AES key and IV are encrypted with the counterparty RSA public key\n    using RSA/ECB/OAEPPadding with SHA-256 OAEP and SHA-256 MGF1. Interchecks publishes its\n    public key in PEM or JWK form via get-encryption-public-key.\n  docs: https://docs-v2.interchecks.com/docs/encrypted-requests\n- name: Webhook signature verification\n  header: x-verification\n  description: >-\n    Inbound webhooks carry an RS256 JWT in the x-verification header whose payload holds iat and\n    request_body_sha256_hash. The verifying public key is fetched by kid from\n    /api/v2/{payer_id}/webhooks/get_validation_key/{kid}.\
  \ Webhooks older than 5 minutes should be\n    rejected.\n  docs: https://docs-v2.interchecks.com/docs/webhooks\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/authentication/interchecks-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Payments
- Payouts
- ACH
- Real-Time Payments
- Instant Payments
- Disbursements
- Cards
- Financial Services
- Fintech
- Webhooks
---
